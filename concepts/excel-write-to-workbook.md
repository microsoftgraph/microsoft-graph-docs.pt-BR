---
title: Gravar dados em uma pasta de trabalho do Excel com o Microsoft Graph
description: q=excelstarter).
ms.localizationpriority: high
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 266427ed2853c26a2267b043b84e04f346467ab2
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60457110"
---
# <a name="write-data-to-an-excel-workbook-with-microsoft-graph"></a>Gravar dados em uma pasta de trabalho do Excel com o Microsoft Graph

A API REST do Excel fornece uma maneira fácil e independente de plataforma de carregar informações em uma pasta de trabalho do Excel. Este tópico mostra como gravar conjuntos de dados simples em uma pasta de trabalho do Excel em três estruturas de desenvolvimento da Web: ASP.NET, Angular e React. Você pode examinar os exemplos de código em destaque neste tópico conferindo [Exemplos do Excel Starter do Microsoft Graph no GitHub](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=excelstarter).

> **Observação:** Todos os três exemplos gravam dados em uma pasta de trabalho do Excel denominada **demo.xlsx**. Elas fornecem esta pasta de trabalho para que você carregar em seu próprio OneDrive, mas você também pode usar o Microsoft Graph para carregar arquivos no OneDrive. Se você tiver interesse em saber quais as chamadas REST você precisa carregar em um arquivo de qualquer tipo na pasta do OneDrive raiz, veja o [exemplo de lista de tarefas pendentes da ASP.NET API do Microsoft Graph Excel](https://github.com/microsoftgraph/aspnet-todo-rest-sample).

Todos os três exemplos do Excel Starter fazem o mesmo: recuperam nome e endereço do usuário conectado e adicionam esses dois tipos de informações a uma nova linha na pasta de trabalho **demo.xlsx**. Você pode modificar os exemplos para adicionar mais linhas, basta adicionar informações à matriz bidimensional que representa a linha ou linhas que você deseja adicionar.

## <a name="add-a-row-or-rows-to-an-excel-workbook-with-a-single-rest-request"></a>Adicionar uma linha ou linhas a uma pasta de trabalho do Excel com uma única solicitação REST

A API REST do Excel exige a postagem de um corpo da solicitação simples para o ponto de extremidade da REST que representa a coleção de linhas de uma pasta de trabalho do Excel. Se você estiver trabalhando com um bloco de anotações na pasta raiz da conta do OneDrive do usuário conectado, o ponto de extremidade REST terá a seguinte aparência:

`https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add`

Para saber mais sobre como acessar arquivos em pastas do OneDrive, confira o [tipo de recurso DriveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) em nossa documentação de referência.

> **Observação:** você pode analisar a coleção de linhas existente da pasta de trabalho fazendo uma solicitação GET para a parte do caminho que termina em `/rows`.

O corpo da POSTAGEM tem a seguinte aparência:

```json
{
  "index": null,
  "values": [
    ["alex darrow", "adarrow@tenant.onmicrosoft.com"]
  ]
}
```

O valor do primeiro parâmetro `index` especifica a posição relativa da linha que você está adicionando à matriz indexada com zero de linhas. As linhas abaixo da linha inserida serão deslocadas para baixo. O parâmetro `null` indica que a nova linha será adicionada ao fim.

O valor do segundo parâmetro `values` é uma matriz de cadeia de caracteres bidimensional que contém os valores não formatados de cada linha que você deseja adicionar. A matriz no exemplo contém apenas uma linha, mas você pode adicionar mais linhas adicionando mais matrizes de cadeia de caracteres.

Você pode testar essa consulta com sua própria conta do OneDrive carregando o arquivo demo.xlsx para sua pasta raiz do OneDrive e executar essa consulta no [Explorador do Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).

Isso é tudo o que você precisa saber para gravar dados em uma pasta de trabalho do Excel. Você precisa saber como criar e fazer a solicitação em sua própria estrutura, e os exemplos do Excel Starter demonstram três maneiras diferentes de fazer isso.

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-aspnet"></a>Adicionar uma linha ou linhas a uma pasta de trabalho do Excel em ASP.NET

Você encontrará o código ASP.NET que cria e envia a solicitação nos arquivos [GraphResources.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphResources.cs) e [GraphService.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphService.cs) do [Exemplo do Excel Starter do Microsoft Graph para ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-excelstarter-sample).

O arquivo `GraphResources.cs` fornece uma classe de ajuda para encapsular dados usuário que você está recuperando do Microsoft Graph e o corpo da solicitação que você usará quando gravar em sua pasta de trabalho.

```csharp
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
```

A classe `GraphService.cs` contém um método `AddInfoToExcel` que popula essas classes, serializa as informações de solicitação em um objeto JSON e passa o objeto como o corpo da solicitação da POSTAGEM.

```csharp
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
```

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-angular"></a>Adicionar uma linha ou linhas a uma pasta de trabalho do Excel em Angular

Você encontrará o código Angular que cria e envia a solicitação no [arquivo home.service.ts](https://github.com/microsoftgraph/angular-excelstarter-sample/blob/master/src/app/home/home.service.ts) do [Exemplo do Excel Starter do Microsoft Graph para Angular](https://github.com/microsoftgraph/angular-excelstarter-sample).

Como este exemplo usa TypeScript, ele tira proveito da [Biblioteca de Cliente de JavaScript do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) e dos [ Tipos TypeScript do Microsoft Graph](https://github.com/microsoftgraph/msgraph-typescript-typings).

A função `addInfoToExcel` no arquivo `home.service.ts` cria a matriz de cadeia de caracteres bidimensional e o corpo da solicitação que contém a matriz. Ela usa então a Biblioteca de Cliente de JavaScript do Microsoft Graph para criar e enviar a solicitação. A resposta volta vem na forma de uma Promessa.

```typescript
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
```

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-react"></a>Adicionar uma linha ou linhas a uma pasta de trabalho do Excel em React

Você encontrará o código que cria e envia a solicitação no [arquivo home.js](https://github.com/microsoftgraph/react-excelstarter-sample/blob/master/src/home/home.js) do [Exemplo do Excel Starter do Microsoft Graph para React](https://github.com/microsoftgraph/react-excelstarter-sample).

A função `onWriteToExcel` cria a matriz de cadeia de caracteres bidimensional e a passa como o corpo da solicitação. Ela usa [axios](https://www.npmjs.com/package/axios) para fazer a solicitação HTTP.

```typescript
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
```

## <a name="see-also"></a>Confira também

* [Gerenciar sessões do Excel usando o Microsoft Graph](excel-manage-sessions.md)
* [Usar funções de pasta de trabalho do Excel com o Microsoft Graph](excel-use-functions.md)
* [Atualizar um formato de intervalo no Excel com o Microsoft Graph](excel-update-range-format.md)
* [Exibir uma imagem do gráfico do Excel com o Microsoft Graph](excel-display-chart-image.md)
* [Usar a API REST do Excel](/graph/api/resources/excel?view=graph-rest-1.0)
