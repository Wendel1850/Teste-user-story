*Exemplo de Código para Teste de Login*

Aqui está um exemplo de código em Java com Selenium WebDriver para testar a funcionalidade de login:
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import org.testng.annotations.Test;

public class LoginTest {
    WebDriver driver = new ChromeDriver();

    @Test
    public void testLoginComSucesso() {
        // Acessar a página de login
        driver.get("https:                      

                                                    
        WebElement usernameInput = driver.findElement(By.name("//example.com/login");

        // Inserir nome de usuário e senha válidos
        WebElement usernameInput = driver.findElement(By.name("username"));
        usernameInput.sendKeys("usuario_valido");
        WebElement passwordInput = driver.findElement(By.name("password"));
        passwordInput.sendKeys("senha_valida");

                                    
        WebElement loginButton = driver.findElement(By.name("// Clicar no botão de login
        WebElement loginButton = driver.findElement(By.name("login"));
        loginButton.click();

                                                                            
        String currentUrl = driver.getCurrentUrl();
        assert currentUrl.equals("// Verificar se o usuário é redirecionado para a página principal
        String currentUrl = driver.getCurrentUrl();
        assert currentUrl.equals("https://example.com/home");
    }

    @Test
    public void testLoginComFalha() {
        // Acessar a página de login
        driver.get("https:                      

                                                      
        WebElement usernameInput = driver.findElement(By.name("//example.com/login");

        // Inserir nome de usuário e senha inválidos
        WebElement usernameInput = driver.findElement(By.name("username"));
        usernameInput.sendKeys("usuario_invalido");
        WebElement passwordInput = driver.findElement(By.name("password"));
        passwordInput.sendKeys("senha_invalida");

                                    
        WebElement loginButton = driver.findElement(By.name("// Clicar no botão de login
        WebElement loginButton = driver.findElement(By.name("login"));
        loginButton.click();

                                                            
        WebElement errorMessage = driver.findElement(By.className("// Verificar se o sistema exibe uma mensagem de erro
        WebElement errorMessage = driver.findElement(By.className("error-message"));
        assert errorMessage.getText().equals("Credenciais inválidas");
    }
}
Esse exemplo de código utiliza o Selenium WebDriver para testar a funcionalidade de login e verificar se o usuário é redirecionado para a página principal após realizar login com sucesso ou se o sistema exibe uma mensagem de erro quando as credenciais são inválidas.
