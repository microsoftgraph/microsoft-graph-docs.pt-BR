---
title: Gravar dados em uma pasta de trabalho do Excel com o Microsoft Graph
description: q=excelstarter).
ms.openlocfilehash: a36e44ce390f0947fbc2d5615551f17becf11b33
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091552"
---
# <a name="write-data-to-an-excel-workbook-with-microsoft-graph"></a><span data-ttu-id="27b2e-103">Gravar dados em uma pasta de trabalho do Excel com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="27b2e-103">Write data to an Excel workbook with Microsoft Graph</span></span>

<span data-ttu-id="27b2e-104">A API REST do Excel fornece uma maneira fácil e independente de plataforma de carregar informações em uma pasta de trabalho do Excel.</span><span class="sxs-lookup"><span data-stu-id="27b2e-104">The Excel REST API provides an easy, platform-agnostic way to upload information to an Excel workbook.</span></span> <span data-ttu-id="27b2e-105">Este tópico mostra como gravar conjuntos de dados simples em uma pasta de trabalho do Excel em três estruturas de desenvolvimento da Web: ASP.NET, Angular e React.</span><span class="sxs-lookup"><span data-stu-id="27b2e-105">This topic shows you how to write simple data sets to an Excel workbook on three web development frameworks: ASP.NET, Angular, and React.</span></span> <span data-ttu-id="27b2e-106">Você pode examinar os exemplos de código em destaque neste tópico conferindo [Exemplos do Excel Starter do Microsoft Graph no GitHub](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=excelstarter).</span><span class="sxs-lookup"><span data-stu-id="27b2e-106">You can look at the code samples featured in this topic by visiting the [Microsoft Graph Excel starter samples on GitHub](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=excelstarter).</span></span>

> <span data-ttu-id="27b2e-107">**Observação:** todos os três exemplos gravam dados em uma pasta de trabalho do Excel denominada **demo.xlxs**.</span><span class="sxs-lookup"><span data-stu-id="27b2e-107">**Note:** All three of the samples write data to an Excel workbook named **demo.xlxs**.</span></span> <span data-ttu-id="27b2e-108">Elas fornecem esta pasta de trabalho para que você carregar em seu próprio OneDrive, mas você também pode usar o Microsoft Graph para carregar arquivos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="27b2e-108">They provide this workbook for you so that you can upload it to your own OneDrive, but you can also use Microsoft Graph to upload files to OneDrive.</span></span> <span data-ttu-id="27b2e-109">Se você tiver interesse em saber quais as chamadas REST você precisa carregar em um arquivo de qualquer tipo na pasta do OneDrive raiz, veja o [exemplo de lista de tarefas pendentes da ASP.NET API do Microsoft Graph Excel](https://github.com/microsoftgraph/aspnet-todo-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="27b2e-109">If you're interested in learning the REST calls you need to upload a file of any type to your root OneDrive folder, see the [Microsoft Graph Excel REST API ASP.NET to-do list sample](https://github.com/microsoftgraph/aspnet-todo-rest-sample).</span></span>

<span data-ttu-id="27b2e-110">Todos os três exemplos do Excel Starter fazem o mesmo: recuperam nome e endereço do usuário conectado e adicionam esses dois tipos de informações a uma nova linha na pasta de trabalho **demo.xlsx**.</span><span class="sxs-lookup"><span data-stu-id="27b2e-110">All three of the Excel starter samples do the same thing: retrieve the name and address of the signed-in user and add those two pieces of information to a new row in the **demo.xlsx** workbook.</span></span> <span data-ttu-id="27b2e-111">Você pode modificar os exemplos para adicionar mais linhas, basta adicionar informações à matriz bidimensional que representa a linha ou linhas que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="27b2e-111">You can modify the samples to add additional rows simply by adding information to the two-dimensional array that represents the row or rows that you want to add.</span></span>

## <a name="add-a-row-or-rows-to-an-excel-workbook-with-a-single-rest-request"></a><span data-ttu-id="27b2e-112">Adicionar uma linha ou linhas a uma pasta de trabalho do Excel com uma única solicitação REST</span><span class="sxs-lookup"><span data-stu-id="27b2e-112">Add a row or rows to an Excel workbook with a single REST request</span></span>

<span data-ttu-id="27b2e-113">A API REST do Excel exige a postagem de um corpo da solicitação simples para o ponto de extremidade da REST que representa a coleção de linhas de uma pasta de trabalho do Excel.</span><span class="sxs-lookup"><span data-stu-id="27b2e-113">The Excel REST API requires you to POST a simple request body to the REST endpoint that represents the row collection of an Excel workbook.</span></span> <span data-ttu-id="27b2e-114">Se você estiver trabalhando com um bloco de anotações na pasta raiz da conta do OneDrive do usuário conectado, o ponto de extremidade REST terá a seguinte aparência:</span><span class="sxs-lookup"><span data-stu-id="27b2e-114">If you're working with a notebook in the root folder of the signed-in user's OneDrive account, the REST endpoint will look like this:</span></span>

`https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add`

<span data-ttu-id="27b2e-115">Para saber mais sobre como acessar arquivos em pastas do OneDrive, confira o [tipo de recurso DriveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) em nossa documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="27b2e-115">For more information about how to reach files in OneDrive folders, see the [DriveItem resource type](/graph/api/resources/driveitem?view=graph-rest-1.0) in our reference documentation.</span></span>

> <span data-ttu-id="27b2e-116">**Observação:** você pode analisar a coleção de linhas existente da pasta de trabalho fazendo uma solicitação GET para a parte do caminho que termina em `/rows`.</span><span class="sxs-lookup"><span data-stu-id="27b2e-116">**Note:** You can look at the existing row collection of the workbook by making a GET request to the part of the path that ends at `/rows`.</span></span>

<span data-ttu-id="27b2e-117">O corpo da POSTAGEM tem a seguinte aparência:</span><span class="sxs-lookup"><span data-stu-id="27b2e-117">The POST body looks like this:</span></span>

`{
  "index": null,
  "values": [
    ['alex darrow', 'adarrow@tenant.onmicrosoft.com']
  ]
}`

<span data-ttu-id="27b2e-118">O valor do primeiro parâmetro `index` especifica a posição relativa da linha que você está adicionando à matriz indexada com zero de linhas.</span><span class="sxs-lookup"><span data-stu-id="27b2e-118">The value of the first `index` parameter specifies the relative position of the row that you're adding to the zero-indexed array of rows.</span></span> <span data-ttu-id="27b2e-119">As linhas abaixo da linha inserida serão deslocadas para baixo.</span><span class="sxs-lookup"><span data-stu-id="27b2e-119">Rows below the inserted row will be shifted downwards.</span></span> <span data-ttu-id="27b2e-120">O parâmetro `null` indica que a nova linha será adicionada ao fim.</span><span class="sxs-lookup"><span data-stu-id="27b2e-120">The `null` parameter indicates that the new row will be added to the end.</span></span>

<span data-ttu-id="27b2e-121">O valor do segundo parâmetro `values` é uma matriz de cadeia de caracteres bidimensional que contém os valores não formatados de cada linha que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="27b2e-121">The value of the second `values` parameter is a two-dimensional string array that contains the unformatted values of each row that you want to add.</span></span> <span data-ttu-id="27b2e-122">A matriz no exemplo contém apenas uma linha, mas você pode adicionar mais linhas adicionando mais matrizes de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="27b2e-122">The array in the sample contains only one row, but you can add more rows by adding more string arrays.</span></span>

<span data-ttu-id="27b2e-123">Você pode testar essa consulta com sua própria conta do OneDrive carregando o arquivo demo.xlsx para sua pasta raiz do OneDrive e executar essa consulta no [Explorador do Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="27b2e-123">You can test this query with your own OneDrive account by uploading the demo.xlsx file to your OneDrive root folder and executing this query on the [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

<span data-ttu-id="27b2e-124">Isso é tudo o que você precisa saber para gravar dados em uma pasta de trabalho do Excel.</span><span class="sxs-lookup"><span data-stu-id="27b2e-124">That is all you need to know in order to write data to an Excel workbook.</span></span> <span data-ttu-id="27b2e-125">Você precisa saber como criar e fazer a solicitação em sua própria estrutura, e os exemplos do Excel Starter demonstram três maneiras diferentes de fazer isso.</span><span class="sxs-lookup"><span data-stu-id="27b2e-125">You do need to know how to construct and make the request in your own framework, and the Excel starter samples demonstrate three separate ways of doing this.</span></span>

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-aspnet"></a><span data-ttu-id="27b2e-126">Adicionar uma linha ou linhas a uma pasta de trabalho do Excel em ASP.NET</span><span class="sxs-lookup"><span data-stu-id="27b2e-126">Add a row or rows to an Excel workbook in ASP.NET</span></span>

<span data-ttu-id="27b2e-127">Você encontrará o código ASP.NET que cria e envia a solicitação nos arquivos [GraphResources.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphResources.cs) e [GraphService.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphService.cs) do [Exemplo do Excel Starter do Microsoft Graph para ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-excelstarter-sample).</span><span class="sxs-lookup"><span data-stu-id="27b2e-127">You'll find the ASP.NET code that constructs and sends the request in the [GraphResources.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphResources.cs) and [GraphService.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphService.cs) files of the [Microsoft Graph Excel Starter Sample for ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-excelstarter-sample).</span></span>

<span data-ttu-id="27b2e-128">O arquivo `GraphResources.cs` fornece uma classe de ajuda para encapsular dados usuário que você está recuperando do Microsoft Graph e o corpo da solicitação que você usará quando gravar em sua pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="27b2e-128">The `GraphResources.cs` file provides a helper class for encapsulating both the user data you're retrieving from Microsoft Graph and the request body that you'll use when you write to your workbook.</span></span>

    public class UserInfo
    {
        public string Name { get; set; }
        public string Address { get; set; }

    }

    public class UserInfoRequest
    {
        public string index { get; set; }
        public string[][] values { get; set; }
    }

<span data-ttu-id="27b2e-129">A classe `GraphService.cs` contém um método `AddInfoToExcel` que popula essas classes, serializa as informações de solicitação em um objeto JSON e passa o objeto como o corpo da solicitação da POSTAGEM.</span><span class="sxs-lookup"><span data-stu-id="27b2e-129">The `GraphService.cs` class contains an `AddInfoToExcel` method that populates these classes, serializes the request information into a JSON object, and then passes that object as the POST request body.</span></span>

        public async Task<string> AddInfoToExcel(string accessToken, string name, string address)
        {
            string endpoint = "https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add";
            using (var client = new HttpClient())
            {
                using (var request = new HttpRequestMessage(HttpMethod.Post, endpoint))
                {
                    // Populate UserInfoRequest object
                    string[] userInfo = { name, address  };
                    string[][] userInfoArray = { userInfo };
                    UserInfoRequest userInfoRequest = new UserInfoRequest();
                    userInfoRequest.index = null;
                    userInfoRequest.values = userInfoArray;

                    // Serialize the information in the UserInfoRequest object
                    string jsonBody = JsonConvert.SerializeObject(userInfoRequest);
                    request.Headers.Accept.Add(new MediaTypeWithQualityHeaderValue("application/json"));
                    request.Headers.Authorization = new AuthenticationHeaderValue("Bearer", accessToken);
                    request.Content = new StringContent(jsonBody, Encoding.UTF8, "application/json");

                    using (var response = await client.SendAsync(request))
                    {
                        if (response.IsSuccessStatusCode)
                        {
                            return Resource.Graph_UploadToExcel_Success_Result;
                        }
                        return response.ReasonPhrase;
                    }
                }
            }
        }

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-angular"></a><span data-ttu-id="27b2e-130">Adicionar uma linha ou linhas a uma pasta de trabalho do Excel em Angular</span><span class="sxs-lookup"><span data-stu-id="27b2e-130">Add a row or rows to an Excel workbook in Angular</span></span>

<span data-ttu-id="27b2e-131">Você encontrará o código Angular que cria e envia a solicitação no [arquivo home.service.ts](https://github.com/microsoftgraph/angular-excelstarter-sample/blob/master/src/app/home/home.service.ts) do [Exemplo do Excel Starter do Microsoft Graph para Angular](https://github.com/microsoftgraph/angular-excelstarter-sample).</span><span class="sxs-lookup"><span data-stu-id="27b2e-131">You'll find the Angular code that constructs and sends the request in the [home.service.ts file](https://github.com/microsoftgraph/angular-excelstarter-sample/blob/master/src/app/home/home.service.ts) of the [Microsoft Graph Excel Starter Sample for Angular](https://github.com/microsoftgraph/angular-excelstarter-sample).</span></span>

<span data-ttu-id="27b2e-132">Como este exemplo usa TypeScript, ele tira proveito da [Biblioteca de Cliente de JavaScript do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) e dos [ Tipos TypeScript do Microsoft Graph](https://github.com/microsoftgraph/msgraph-typescript-typings).</span><span class="sxs-lookup"><span data-stu-id="27b2e-132">Since this sample uses TypeScript, it takes advantage of the [Microsoft Graph JavaScript Client Library](https://github.com/microsoftgraph/msgraph-sdk-javascript) and the [ Microsoft Graph TypeScript Types](https://github.com/microsoftgraph/msgraph-typescript-typings).</span></span>

<span data-ttu-id="27b2e-133">A função `addInfoToExcel` no arquivo `home.service.ts` cria a matriz de cadeia de caracteres bidimensional e o corpo da solicitação que contém a matriz.</span><span class="sxs-lookup"><span data-stu-id="27b2e-133">The `addInfoToExcel` function in the `home.service.ts` file constructs the two-dimensional string array and the request body that contains the array.</span></span> <span data-ttu-id="27b2e-134">Ela usa então a Biblioteca de Cliente de JavaScript do Microsoft Graph para criar e enviar a solicitação.</span><span class="sxs-lookup"><span data-stu-id="27b2e-134">It then uses the Microsoft Graph JavaScript Client Library to construct and send the request.</span></span> <span data-ttu-id="27b2e-135">A resposta volta vem na forma de uma Promessa.</span><span class="sxs-lookup"><span data-stu-id="27b2e-135">The response comes back in the form of a Promise.</span></span>

      addInfoToExcel(user: MicrosoftGraph.User) {
        const userInfo = [];
        const userEmail = user.mail || user.userPrincipalName;    
        userInfo.push([user.displayName, userEmail]);

        const userInfoRequestBody = {
          index: null,
          values: userInfo
        };   

        const body = JSON.stringify(userInfoRequestBody);

        var client = this.getClient();
        var url = `${this.url}/me/drive/root:/${this.file}:/workbook/tables/${this.table}/rows/add`
        return Observable.fromPromise(client
        .api(url)
        .post(body)
        );
      }

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-react"></a><span data-ttu-id="27b2e-136">Adicionar uma linha ou linhas a uma pasta de trabalho do Excel em React</span><span class="sxs-lookup"><span data-stu-id="27b2e-136">Add a row or rows to an Excel workbook in React</span></span>

<span data-ttu-id="27b2e-137">Você encontrará o código que cria e envia a solicitação no [arquivo home.js](https://github.com/microsoftgraph/react-excelstarter-sample/blob/master/src/home/home.js) do [Exemplo do Excel Starter do Microsoft Graph para React](https://github.com/microsoftgraph/react-excelstarter-sample).</span><span class="sxs-lookup"><span data-stu-id="27b2e-137">You'll find the code that constructs and sends the request in the [home.js file](https://github.com/microsoftgraph/react-excelstarter-sample/blob/master/src/home/home.js) of the [Microsoft Graph Excel Starter Sample for React](https://github.com/microsoftgraph/react-excelstarter-sample).</span></span>

<span data-ttu-id="27b2e-138">A função `onWriteToExcel` cria a matriz de cadeia de caracteres bidimensional e a passa como o corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27b2e-138">The `onWriteToExcel` function constructs the two-dimensional string array and passes it as the request body.</span></span> <span data-ttu-id="27b2e-139">Ela usa [axios](https://www.npmjs.com/package/axios) para fazer a solicitação HTTP.</span><span class="sxs-lookup"><span data-stu-id="27b2e-139">It uses [axios](https://www.npmjs.com/package/axios) to make the HTTP request.</span></span>

      onWriteToExcel() {
        const { token, me } = this.state;

        const myEmailAddress = me.mail || me.userPrincipalName;
        const values = [];

        values.push([me.displayName, myEmailAddress]);

        axios
          .post('https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add',
            { index: null, values },
            { headers: { Authorization: `Bearer ${token}` }}
          )
          .then(res => {
                          console.log(res);
                          const successMessage = "Successfully wrote your data to demo.xlsx!";
                          this.setState ({ successMessage });
                         })
          .catch(err => console.error(err));
      }

##<a name="see-also"></a><span data-ttu-id="27b2e-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="27b2e-140">See also</span></span>

* [<span data-ttu-id="27b2e-141">Gerenciar sessões do Excel usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="27b2e-141">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="27b2e-142">Usar funções de pasta de trabalho do Excel com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="27b2e-142">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="27b2e-143">Atualizar um formato de intervalo no Excel com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="27b2e-143">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="27b2e-144">Exibir uma imagem do gráfico do Excel com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="27b2e-144">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="27b2e-145">Usar a API REST do Excel</span><span class="sxs-lookup"><span data-stu-id="27b2e-145">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)    
