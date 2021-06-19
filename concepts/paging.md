---
title: 'Paginação de dados do Microsoft Graph em seu aplicativo '
description: 'Propriedade odata.nextLink` na resposta que contém uma URL para a próxima página de resultados. '
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: be2d927de3cf1f3d419d7daa5747e0cc9e70c28c
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030877"
---
# <a name="paging-microsoft-graph-data-in-your-app"></a><span data-ttu-id="14829-103">Paginação de dados do Microsoft Graph em seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="14829-103">Paging Microsoft Graph data in your app</span></span> 

<span data-ttu-id="14829-p101">Algumas consultas em relação ao Microsoft Graph retornam várias páginas de dados devido à paginação do lado do servidor ou devido ao uso do parâmetro de consulta `$top` para limitar especificamente o tamanho da página em uma solicitação. Quando um conjunto de resultados se estende por várias páginas, o Microsoft Graph retorna uma propriedade `@odata.nextLink` na resposta que contém uma URL para a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="14829-p101">Some queries against Microsoft Graph return multiple pages of data either due to server-side paging or due to the use of the `$top` query parameter to specifically limit the page size in a request. When a result set spans multiple pages, Microsoft Graph returns an `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> 

<span data-ttu-id="14829-106">Por exemplo, a URL a seguir solicita todos os usuários em uma organização com o tamanho de página 5 especificado com o parâmetro de consulta `$top`:</span><span class="sxs-lookup"><span data-stu-id="14829-106">For example, the following URL requests all the users in an organization with a page size of 5, specified with the `$top` query parameter:</span></span>

```html
https://graph.microsoft.com/v1.0/users?$top=5
```

<span data-ttu-id="14829-107">Se o resultado contiver mais de cinco usuários, o Microsoft Graph retornará uma propriedade `@odata.nextLink` semelhante à mostrada a seguir, junto com a primeira página de usuários.</span><span class="sxs-lookup"><span data-stu-id="14829-107">If the result contains more than five users, Microsoft Graph will return an `@odata.nextLink` property similar to the following along with the first page of users.</span></span>

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27"
```

<span data-ttu-id="14829-108">Você pode recuperar a próxima página de resultados enviando o valor de URL da propriedade `@odata.nextLink` para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="14829-108">You can retrieve the next page of results by sending the URL value of the `@odata.nextLink` property to Microsoft Graph.</span></span> 

```html
https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27
```

<span data-ttu-id="14829-109">O Microsoft Graph continuará a retornar uma referência para a próxima página de dados na propriedade `@odata.nextLink` com cada resposta até que todas as páginas do resultado sejam lidas.</span><span class="sxs-lookup"><span data-stu-id="14829-109">Microsoft Graph will continue to return a reference to the next page of data in the `@odata.nextLink` property with each response until all pages of the result have been read.</span></span>

><span data-ttu-id="14829-110">**Importante:** Você deve incluir a URL inteira na propriedade `@odata.nextLink` na solicitação da próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="14829-110">**Important:** You should include the entire URL in the `@odata.nextLink` property in your request for the next page of results.</span></span> <span data-ttu-id="14829-111">Dependendo da API em relação à qual a consulta está sendo realizada, o valor de URL `@odata.nextLink` conterá um parâmetro de consulta `$skiptoken` ou `$skip`.</span><span class="sxs-lookup"><span data-stu-id="14829-111">Depending on the API that the query is being performed against, the `@odata.nextLink` URL value will contain either a `$skiptoken` or a `$skip` query parameter.</span></span> <span data-ttu-id="14829-112">A URL também contém todos os outros parâmetros de consulta presentes na solicitação original.</span><span class="sxs-lookup"><span data-stu-id="14829-112">The URL also contains all the other query parameters present in the original request.</span></span> <span data-ttu-id="14829-113">Não tente extrair o valor `$skiptoken` ou `$skip` e usá-lo em uma solicitação diferente.</span><span class="sxs-lookup"><span data-stu-id="14829-113">Do not try to extract the `$skiptoken` or `$skip` value and use it in a different request.</span></span> 

<span data-ttu-id="14829-114">O comportamento de paginação varia entre diferentes APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="14829-114">Paging behavior varies across different Microsoft Graph APIs.</span></span> <span data-ttu-id="14829-115">Ao trabalhar com dados paginados, considere o seguinte:</span><span class="sxs-lookup"><span data-stu-id="14829-115">Consider the following when working with paged data:</span></span>

- <span data-ttu-id="14829-116">APIs diferentes podem ter tamanhos padrão e máximo de página diferentes.</span><span class="sxs-lookup"><span data-stu-id="14829-116">Different APIs might have different default and maximum page sizes.</span></span>
- <span data-ttu-id="14829-117">APIs diferentes poderão se comportar de maneira diferente se você especificar um tamanho de página (por meio do parâmetro de consulta `$top`) que exceda o tamanho máximo de página para essa API.</span><span class="sxs-lookup"><span data-stu-id="14829-117">Different APIs might behave differently if you specify a page size (via the `$top` query parameter) that exceeds the maximum page size for that API.</span></span> <span data-ttu-id="14829-118">Dependendo da API, o tamanho de página solicitado pode ser ignorado, ele pode usar por padrão o tamanho máximo de página para essa API ou o Microsoft Graph pode retornar um erro.</span><span class="sxs-lookup"><span data-stu-id="14829-118">Depending on the API, the requested page size might be ignored, it might default to the maximum page size for that API, or Microsoft Graph might return an error.</span></span> 
- <span data-ttu-id="14829-p105">Nem todos os recursos ou relações dão suporte à paginação. Por exemplo, consultas em relação a [directoryRoles](/graph/api/resources/directoryrole) não dão suporte à paginação. Isso inclui os objetos de função de leitura e os membros de função.</span><span class="sxs-lookup"><span data-stu-id="14829-p105">Not all resources or relationships support paging. For example, queries against [directoryRoles](/graph/api/resources/directoryrole) do not support paging. This includes reading role objects themselves as well as role members.</span></span>
- <span data-ttu-id="14829-122">Ao fazer paginação em recursos de diretório, quaisquer cabeçalhos de solicitação adicionais, como o cabeçalho **ConsistencyLevel**, não são incluídos por padrão em solicitações de página subsequentes.</span><span class="sxs-lookup"><span data-stu-id="14829-122">When paging against directory resources, any additional request headers such as the **ConsistencyLevel** header are not included by default in subsequent page requests.</span></span> <span data-ttu-id="14829-123">Se esses cabeçalhos precisam ser enviados em solicitações subsequentes, você deve defini-los explicitamente.</span><span class="sxs-lookup"><span data-stu-id="14829-123">If those headers need to be sent on subsequent requests, you must set them explicitly.</span></span>
- <span data-ttu-id="14829-124">Ao usar a cadeia de consulta `$count=true` ao consultar recursos de diretório, a propriedade `@odata.count` estará presente apenas na primeira página dos dados paginados.</span><span class="sxs-lookup"><span data-stu-id="14829-124">When using the `$count=true` query string when querying against directory resources, the `@odata.count` property will be present only in the first page of the paged data.</span></span>

## <a name="learn-more-about-paging"></a><span data-ttu-id="14829-125">Saiba mais sobre paginação</span><span class="sxs-lookup"><span data-stu-id="14829-125">Learn more about paging</span></span>
<span data-ttu-id="14829-126">O vídeo a seguir apresenta a paginação no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="14829-126">The following video introduces you to paging in Microsoft Graph.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/DB_NoC9a1JI]
