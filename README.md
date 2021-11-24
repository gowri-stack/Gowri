# Gowri
Search functionality

-----------------------------
Go to selenium
- Create a new class
- Copy paste this code: 
------------------------------------------------------
import org.openqa.selenium.By;
import org.openqa.selenium.Keys;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;

public class JTC {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		System.setProperty("webdriver.chrome.driver", "C:\\chrome95\\chromedriver.exe");
		WebDriver driver = new ChromeDriver();
		driver.get("https://google.com/");
		driver.manage().window().maximize();
		WebElement element = driver.findElement(By.name("q"));
		element.sendKeys("Books");
		element.submit();
		driver.close();
		
	}

}
-----------------------------------------------------------------------
Right click -> Run as -> Java application 
