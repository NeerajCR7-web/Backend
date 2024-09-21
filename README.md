# Backend
using Microsoft.AspNetCore.Http;
using Microsoft.AspNetCore.Mvc;

namespace Assignment1.Controllers
{
    [Route("api/[controller]")]
    [ApiController]
    public class TestController : ControllerBase
    {
        // GET localhost:xx/api/test/method1 -> "Hello World"
        [HttpGet(template:"Method1")]
        public string Method1()
        {
            return "Hello World";