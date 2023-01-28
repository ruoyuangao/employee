# employee


controller
service -> resttemplate -> request -> https://reqres.in/api/users


1. config resttemplate bean in configuration 
2. autowired resttemplate in service layer
3. resttemplate.getForObject(url, A.class) / resttemplate.getForObject(url, Map.class)
 
class A {
 List<B> data;
}
class B {}
4. return result to controller
 /employees => group by ages
 {
  22: [{}, {}, {}],
  61: [{}, {}, {}]
 }
 /employees?age=xx => emp’s ages > xx
 {
  “data”: [{}, {}, {}]
 }
