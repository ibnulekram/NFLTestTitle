# NFLTestTitle
import junit.framework.Assert;

import org.junit.Test;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.firefox.FirefoxDriver;
public class NFLTest

{
@Test
public void TestTitle()

{
WebDriver dr= new FirefoxDriver();
dr.get("http://scores.espn.go.com/nfl/scoreboard");

String ptitle=dr.getTitle();
Assert.assertTrue("Title not found!", ptitle.contains("NFL Scoreboard"));

}
}
