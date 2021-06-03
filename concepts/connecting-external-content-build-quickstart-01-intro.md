<!-- markdownlint-disable MD002 MD025 MD041 -->
<!--- # Introduction --->

<span data-ttu-id="1a428-101">Os conectores Graph Microsoft permitem que você adicione seus próprios dados ao Microsoft Graph e que ele acione várias Microsoft 365 experiências.</span><span class="sxs-lookup"><span data-stu-id="1a428-101">Microsoft Graph connectors allow you to add your own data into Microsoft Graph and have it power various Microsoft 365 experiences.</span></span>

<span data-ttu-id="1a428-102">Este aplicativo .NET Core mostra como usar a API de conectores do Microsoft Graph para criar um conector de cliente e usá-lo para a Pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1a428-102">This .NET Core application shows you how to use the Microsoft Graph connectors API to create a customer connector and use it to power Microsoft Search.</span></span> <span data-ttu-id="1a428-103">Este tutorial usa um exemplo de inventário de partes de dispositivos de dados para a organização De reparo de dispositivos contoso.</span><span class="sxs-lookup"><span data-stu-id="1a428-103">This tutorial uses a sample data appliance parts inventory for the Contoso Appliance Repair organization.</span></span>

## <a name="how-does-the-sample-work"></a><span data-ttu-id="1a428-104">Como funciona o exemplo?</span><span class="sxs-lookup"><span data-stu-id="1a428-104">How does the sample work?</span></span>

<span data-ttu-id="1a428-105">O exemplo cria um Windows da área de trabalho que adquire um token do plataforma de identidade da Microsoft e o usa para enviar solicitações para a API de conectores Graph Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1a428-105">The sample creates a Windows desktop app that acquires a token from the Microsoft identity platform, and uses it to send requests to the Microsoft Graph connectors API.</span></span> <span data-ttu-id="1a428-106">A API de conectores enviará sua resposta depois que o acesso for validado.</span><span class="sxs-lookup"><span data-stu-id="1a428-106">The connectors API will send its response after the access is validated.</span></span>

![Diagrama mostrando o aplicativo Windows adquirir um token e usá-lo para acessar a API de conectores Graph Microsoft](images/connectors-images/build1.png)

## <a name="prerequisites"></a><span data-ttu-id="1a428-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1a428-108">Prerequisites</span></span>

* <span data-ttu-id="1a428-109">Instale [Visual Studio 2019](https://visualstudio.microsoft.com/) com [o .NET Core 3.1 SDK](https://www.microsoft.com/net/download/core) em seu computador de desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="1a428-109">Install [Visual Studio 2019](https://visualstudio.microsoft.com/) with [.NET Core 3.1 SDK](https://www.microsoft.com/net/download/core) on your development computer.</span></span>
* <span data-ttu-id="1a428-110">Certifique-se de ter uma [conta pessoal da Microsoft](https://signup.live.com/)ou uma conta de estudante ou de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1a428-110">Make sure that you have a [personal Microsoft account](https://signup.live.com/), or a work or school account.</span></span>
* <span data-ttu-id="1a428-111">Instale as Ferramentas Principais da Estrutura de [Entidades](/ef/core/miscellaneous/cli/dotnet) como uma ferramenta global usando o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="1a428-111">Install the [Entity Framework Core Tools](/ef/core/miscellaneous/cli/dotnet) as a global tool using the following command:</span></span>

    ```dotnetcli
    dotnet tool install --global dotnet-ef
    ```

* <span data-ttu-id="1a428-112">Instale uma ferramenta para atualizar um banco de dados SQLite.</span><span class="sxs-lookup"><span data-stu-id="1a428-112">Install a tool to update a SQLite database.</span></span> <span data-ttu-id="1a428-113">Por exemplo, o [Navegador DB para SQLite](https://sqlitebrowser.org/).</span><span class="sxs-lookup"><span data-stu-id="1a428-113">For example, the [DB Browser for SQLite](https://sqlitebrowser.org/).</span></span>
* <span data-ttu-id="1a428-114">Baixe o **ApplianceParts.csv** do repo de exemplo [do conector de pesquisa.](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/PartsInventoryConnector/ApplianceParts.csv)</span><span class="sxs-lookup"><span data-stu-id="1a428-114">Download the **ApplianceParts.csv** file from the [Search connector sample repo](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/PartsInventoryConnector/ApplianceParts.csv).</span></span>

> [!TIP]
> <span data-ttu-id="1a428-115">A melhor maneira de baixar arquivos GitHub é ir para o nível superior do projeto.</span><span class="sxs-lookup"><span data-stu-id="1a428-115">The best way to download files from GitHub is to go to the top level of the project.</span></span> <span data-ttu-id="1a428-116">No botão de download **de código** verde à direita, escolha **Baixar ZIP**.</span><span class="sxs-lookup"><span data-stu-id="1a428-116">From the green **Code** download button on the right, choose **Download ZIP**.</span></span> <span data-ttu-id="1a428-117">O arquivo ZIP conterá o conteúdo do repositório.</span><span class="sxs-lookup"><span data-stu-id="1a428-117">The ZIP file will contain the contents of the repository.</span></span>
