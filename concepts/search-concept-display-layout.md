---
ms.author: yiwenwang
title: Usar a API Pesquisa da Microsoft no Microsoft Graph renderizar o layout de exibição
description: Use a API Pesquisa da Microsoft no Microsoft Graph para exibir os resultados da pesquisa de maneiras diferentes.
author: yiwenwang
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 4f58e7b4a303ba6b20b1d70bd765b38d1526bbca
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211159"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-render-display-layout-preview"></a><span data-ttu-id="4094f-103">Use a API Pesquisa da Microsoft no Microsoft Graph renderizar layout de exibição (visualização)</span><span class="sxs-lookup"><span data-stu-id="4094f-103">Use the Microsoft Search API in Microsoft Graph to render display layout (preview)</span></span>

<span data-ttu-id="4094f-104">Um layout de exibição de pesquisa ou tipo de resultado é uma regra que faz com que tipos distintos de resultados de pesquisa sejam exibidos de maneiras diferentes nas páginas de resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4094f-104">A search display layout or result type is a rule that causes distinct kinds of search results to be displayed in different ways in search result pages.</span></span> <span data-ttu-id="4094f-105">Ele consiste no seguinte:</span><span class="sxs-lookup"><span data-stu-id="4094f-105">It consists of the following:</span></span> 

- <span data-ttu-id="4094f-106">Uma ou mais características ou condições para comparar cada resultado de pesquisa, como a fonte de resultados ou o tipo de conteúdo do resultado da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4094f-106">One or more characteristics or conditions to compare each search result against, such as the result source or content type of the search result.</span></span>
- <span data-ttu-id="4094f-p102">O modelo de exibição pesquisa os resultados que atendem às condições. O modelo de exibição controla a forma que os resultados que correspondem às condições serão exibidos e se comportarão na página dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4094f-p102">A display template to use for search results that meet the conditions. The display template controls the way in which all results that meet the conditions appear and behave on a search results page.</span></span> 

<span data-ttu-id="4094f-109">A API Graph de Pesquisa da Microsoft fornece uma resposta renderizável com base em [Cartões Adaptáveis.](https://adaptivecards.io/)</span><span class="sxs-lookup"><span data-stu-id="4094f-109">The Microsoft Graph Search API provides a renderable response based on [Adaptive Cards](https://adaptivecards.io/).</span></span> <span data-ttu-id="4094f-110">Usando o modelo [cartão adaptável,](https://adaptivecards.io/designer)os clientes podem renderizar diferentes resultados de pesquisa em diferentes telas.</span><span class="sxs-lookup"><span data-stu-id="4094f-110">By using the [Adaptive Card template](https://adaptivecards.io/designer), clients can render different search result in different canvases.</span></span>

<span data-ttu-id="4094f-111">Os clientes podem personalizar o tipo de resultado de pesquisa no [Centro de administração do Microsoft 365](https://admin.microsoft.com/Adminportal/Home#/MicrosoftSearch/resulttypes).</span><span class="sxs-lookup"><span data-stu-id="4094f-111">Customers can customize their search result type in the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home#/MicrosoftSearch/resulttypes).</span></span>

## <a name="request-example"></a><span data-ttu-id="4094f-112">Exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="4094f-112">Request example</span></span>

<span data-ttu-id="4094f-113">O exemplo a seguir mostra como obter os layouts de exibição ou modelos de resultados para renderizar os resultados da pesquisa definindo a **propriedade enableResultTemplate** como no `true` contrato de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4094f-113">The following example shows how to get the display layouts or result templates for rendering the search results by setting the **enableResultTemplate** property to `true` in the request contract.</span></span>

<span data-ttu-id="4094f-114">A reponse mostra três visitas de pesquisa, duas delas relacionadas, com o **resultTemplateId** 1603900360618_5XCBK2OXG e a outra com o **resultTemplateId** 1603900360618_5XCBK2OXP.</span><span class="sxs-lookup"><span data-stu-id="4094f-114">The reponse shows three search hits, two of them related, with the **resultTemplateId** 1603900360618_5XCBK2OXG, and the other one with the **resultTemplateId** 1603900360618_5XCBK2OXP.</span></span> <span data-ttu-id="4094f-115">Essas IDs combinam com uma das chaves dos dois layouts de exibição contidos no dicionário **resultTemplates** incluído no contrato de resposta.</span><span class="sxs-lookup"><span data-stu-id="4094f-115">These IDs match with one of the keys of the two display layouts contained in the **resultTemplates** dictionary that's included within the response contract.</span></span> <span data-ttu-id="4094f-116">Usando as IDs do modelo de resultado, você pode determinar qual layout de exibição usar para renderizar cada resultado da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4094f-116">Using the result template IDs, you can determine which display layout to use to render each search result.</span></span>

### <a name="request"></a><span data-ttu-id="4094f-117">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4094f-117">Request</span></span>

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
Content-Type: application/json

{
    "requests": [
        {
            "entityTypes": [
                "externalItem"
            ],
            "contentSources": [
                "Connectors"
            ],
            "query": {
                "queryString": "*"
            },
            "resultTemplateOptions": {
                "enableResultTemplate": true
            }
        }
    ]
}
```

### <a name="response"></a><span data-ttu-id="4094f-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="4094f-118">Response</span></span>


```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.searchResponse)",
    "value": [
        {
            "searchTerms": [],
            "hitsContainers": [
                {
                    "total": 1201701,
                    "moreResultsAvailable": true,
                    "hits": [
                        {
                            "hitId": "85437765-b430-434f-a945-38eceead5b93",
                            "rank": 1,
                            "summary": "",
                            "resultTemplateId": "1603900360618_5XCBK2OXG",
                            "resource": {
                                "@odata.type": "#microsoft.graph.externalItem",
                                "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17397",
                                "Title": "[SM00186] Number of tests - Liquid",
                                "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                            }
                        },
                        {
                            "hitId": "85437765-5430-434f-a945-38eceead5b94",
                            "rank": 2,
                            "summary": "",
                            "resultTemplateId": "1603900360618_5XCBK2OXP",
                            "resource": {
                                "@odata.type": "#microsoft.graph.externalItem",
                                "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17398",
                                "Title": "[SM00186] Number of tests - Liquid 2",
                                "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                            }
                        },
                        {
                            "hitId": "85437765-b430-434f-a945-38eceead5b95",
                            "rank": 3,
                            "summary": "",
                            "resultTemplateId": "1603900360618_5XCBK2OXG",
                            "resource": {
                                "@odata.type": "#microsoft.graph.externalItem",
                                "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17399",
                                "Title": "[SM00186] Number of tests - Liquid 3",
                                "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                            }
                        }
                    ]
                }
            ],
            "resultTemplates": {
                "1603900360618_5XCBK2OXG": {
                    "displayName": "Liquid-3",
                    "body": {
                        "type": "AdaptiveCard",
                        "version": "1.0",
                        "body": [
                            {
                                "type": "ColumnSet",
                                "columns": [
                                    {
                                        "type": "Column",
                                        "width": "auto",
                                        "items": [
                                            {
                                                "type": "Image",
                                                "url": "https://searchuxcdn.azureedge.net/designerapp/images/LiquidLogo.png",
                                                "horizontalAlignment": "Center",
                                                "size": "Small"
                                            }
                                        ],
                                        "horizontalAlignment": "Center"
                                    },
                                    {
                                        "type": "Column",
                                        "width": 10,
                                        "items": [
                                            {
                                                "type": "TextBlock",
                                                "text": "[{Title}]({URL})",
                                                "weight": "Bolder",
                                                "color": "Accent",
                                                "size": "Medium",
                                                "maxLines": 3
                                            },
                                            {
                                                "type": "TextBlock",
                                                "text": "{ResultSnippet}",
                                                "maxLines": 3,
                                                "wrap": true
                                            }
                                        ],
                                        "spacing": "Medium"
                                    }
                                ]
                            }
                        ],
                        "$schema": "http://adaptivecards.io/schemas/adaptive-card.json"
                    }
                },
                "1603900360618_5XCBK2OXP": {
                    "displayName": "Liquid-2",
                    "body": {
                        "type": "AdaptiveCard",
                        "version": "1.0",
                        "body": [
                            {
                                "type": "ColumnSet",
                                "columns": [
                                    {
                                        "type": "Column",
                                        "width": "auto",
                                        "items": [
                                            {
                                                "type": "Image",
                                                "url": "https://searchuxcdn.azureedge.net/designerapp/images/LiquidLogo.png",
                                                "horizontalAlignment": "Center",
                                                "size": "Small"
                                            }
                                        ],
                                        "horizontalAlignment": "Center"
                                    },
                                    {
                                        "type": "Column",
                                        "width": 10,
                                        "items": [
                                            {
                                                "type": "TextBlock",
                                                "text": "[{Title}]({URL})",
                                                "weight": "Bolder",
                                                "color": "Accent",
                                                "size": "Medium",
                                                "maxLines": 3
                                            },
                                            {
                                                "type": "TextBlock",
                                                "text": "{ResultSnippet}",
                                                "maxLines": 3,
                                                "wrap": true
                                            }
                                        ],
                                        "spacing": "Medium"
                                    }
                                ]
                            }
                        ],
                        "$schema": "http://adaptivecards.io/schemas/adaptive-card.json"
                    }
                }
            }
        }
    ]
}

```

## <a name="web-component-example"></a><span data-ttu-id="4094f-119">Exemplo de componente web</span><span class="sxs-lookup"><span data-stu-id="4094f-119">Web component example</span></span>

<span data-ttu-id="4094f-120">O exemplo a seguir mostra como usar a tentação de Cartão Adaptável para renderizar os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4094f-120">The following example shows how to use Adaptive Card templating to render search results.</span></span>

> [!IMPORTANT] 
> 
> <span data-ttu-id="4094f-121">Este exemplo usa uma versão do Cartão Adaptável emplacar anteriormente à versão de maio de **2020.**</span><span class="sxs-lookup"><span data-stu-id="4094f-121">This example uses a version of Adaptive Card templating earlier than the **May 2020 release**.</span></span> <span data-ttu-id="4094f-122">Para saber mais, consulte:</span><span class="sxs-lookup"><span data-stu-id="4094f-122">For more details, see:</span></span>
> - [<span data-ttu-id="4094f-123">Templating de cartão adaptável</span><span class="sxs-lookup"><span data-stu-id="4094f-123">Adaptive Card templating</span></span>](/adaptive-cards/templating/)
> - [<span data-ttu-id="4094f-124">SDK de templating de cartão adaptável</span><span class="sxs-lookup"><span data-stu-id="4094f-124">Adaptive Card templating SDK</span></span>](/adaptive-cards/templating/sdk)


<!-- markdownlint-disable MD024 -->
```HTML
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="utf-8" />
    <title>Adaptive Cards Example</title>

    <script src="https://unpkg.com/markdown-it@8.4.0/dist/markdown-it.js"></script>
    <script src="https://unpkg.com/adaptivecards/dist/adaptivecards.min.js"></script>

    <script src="https://unpkg.com/adaptivecards-templating@0.1.0-alpha1/dist/adaptivecards-templating.min.js"></script>
    <script src="https://code.jquery.com/jquery-3.6.0.js"
        integrity="sha256-H+K7U5CnXl1h5ywQfKtSj8PCmoN9aaq30gDh27Xc0jk=" crossorigin="anonymous"></script>

    <style type="text/css">
        #exampleDiv {
            border: solid 1px black;
        }
    </style>

    <script type="text/javascript">

       function renderCard() {
            var mockdata = this.getMockData();
            var renderTemplates = [];

            // Convert object to map
            var templateDictionary = new Map(Object.entries( mockdata.value[0].resultTemplates));

            for (let hit of mockdata.value[0].hitsContainers[0].hits) {
                renderTemplates.push(this.renderACT(hit, templateDictionary));
            }

            for(let template of renderTemplates){
                document.getElementById('exampleDiv').appendChild(template);
            }
        }

        function renderACT(hit, templateDictionary) {
            var templateId = hit.resultTemplateId;
            // Define a template payload
            var templatePayload = templateDictionary.get(templateId).body;
            var template = new ACData.Template(templatePayload);

            // Expand the template with your `$root` data object.
            // This binds it to the data and produces the final Adaptive Card payload

            console.log(hit.resource);

            // Create a data binding context, and set its $root property to the
            // data object to bind the template to
            var context = new ACData.EvaluationContext();
            context.$root = hit.resource;

            console.log(context);
            var card = template.expand(context);
            // OPTIONAL: Render the card (requires that the adaptivecards library be loaded)

            var adaptiveCard = new AdaptiveCards.AdaptiveCard();
            adaptiveCard.parse(card);
            return adaptiveCard.render();
        }

        function getMockData() {
            return {
                "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.searchResponse)",
                "value": [
                    {
                        "searchTerms": [],
                        "hitsContainers": [
                            {
                                "total": 1201701,
                                "moreResultsAvailable": true,
                                "hits": [
                                    {
                                        "hitId": "85437765-b430-434f-a945-38eceead5b93",
                                        "rank": 1,
                                        "summary": "",
                                        "resultTemplateId": "1603900360618_5XCBK2OXG",
                                        "resource": {
                                            "@odata.type": "#microsoft.graph.externalItem",
                                            "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17397",
                                            "Title": "[SM00186] Number of tests - Liquid",
                                            "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                                        }
                                    },
                                    {
                                        "hitId": "85437765-5430-434f-a945-38eceead5b94",
                                        "rank": 2,
                                        "summary": "",
                                        "resultTemplateId": "1603900360618_5XCBK2OXP",
                                        "resource": {
                                            "@odata.type": "#microsoft.graph.externalItem",
                                            "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17398",
                                            "Title": "[SM00186] Number of tests - Liquid 2",
                                            "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                                        }
                                    },
                                    {
                                        "hitId": "85437765-b430-434f-a945-38eceead5b95",
                                        "rank": 3,
                                        "summary": "",
                                        "resultTemplateId": "1603900360618_5XCBK2OXG",
                                        "resource": {
                                            "@odata.type": "#microsoft.graph.externalItem",
                                            "id": "B5B6E9C7-152C-4478-BCCB-CEF053F17399",
                                            "Title": "[SM00186] Number of tests - Liquid 3",
                                            "URL": "https://liquid.microsoft.com/Web/Object/Read/scanningtoolwarnings/Requirements/CodeQL.SM00186"
                                        }
                                    }
                                ]
                            }
                        ],
                        "resultTemplates": {
                            "1603900360618_5XCBK2OXG": {
                                "displayName": "Liquid-3",
                                "body": {
                                    "type": "AdaptiveCard",
                                    "version": "1.0",
                                    "body": [
                                        {
                                            "type": "ColumnSet",
                                            "columns": [
                                                {
                                                    "type": "Column",
                                                    "width": "auto",
                                                    "items": [
                                                        {
                                                            "type": "Image",
                                                            "url": "https://searchuxcdn.azureedge.net/designerapp/images/LiquidLogo.png",
                                                            "horizontalAlignment": "Center",
                                                            "size": "Small"
                                                        }
                                                    ],
                                                    "horizontalAlignment": "Center"
                                                },
                                                {
                                                    "type": "Column",
                                                    "width": 10,
                                                    "items": [
                                                        {
                                                            "type": "TextBlock",
                                                            "text": "[{Title}]({URL})",
                                                            "weight": "Bolder",
                                                            "color": "Accent",
                                                            "size": "Medium",
                                                            "maxLines": 3
                                                        },
                                                        {
                                                            "type": "TextBlock",
                                                            "text": "{ResultSnippet}",
                                                            "maxLines": 3,
                                                            "wrap": true
                                                        }
                                                    ],
                                                    "spacing": "Medium"
                                                }
                                            ]
                                        }
                                    ],
                                    "$schema": "http://adaptivecards.io/schemas/adaptive-card.json"
                                }
                            },
                            "1603900360618_5XCBK2OXP": {
                                "displayName": "Liquid-2",
                                "body": {
                                    "type": "AdaptiveCard",
                                    "version": "1.0",
                                    "body": [
                                        {
                                            "type": "ColumnSet",
                                            "columns": [
                                                {
                                                    "type": "Column",
                                                    "width": "auto",
                                                    "items": [
                                                        {
                                                            "type": "Image",
                                                            "url": "https://searchuxcdn.azureedge.net/designerapp/images/LiquidLogo.png",
                                                            "horizontalAlignment": "Center",
                                                            "size": "Small"
                                                        }
                                                    ],
                                                    "horizontalAlignment": "Center"
                                                },
                                                {
                                                    "type": "Column",
                                                    "width": 10,
                                                    "items": [
                                                        {
                                                            "type": "TextBlock",
                                                            "text": "[{Title}]({URL})",
                                                            "weight": "Bolder",
                                                            "color": "Accent",
                                                            "size": "Medium",
                                                            "maxLines": 3
                                                        },
                                                        {
                                                            "type": "TextBlock",
                                                            "text": "{ResultSnippet}",
                                                            "maxLines": 3,
                                                            "wrap": true
                                                        }
                                                    ],
                                                    "spacing": "Medium"
                                                }
                                            ]
                                        }
                                    ],
                                    "$schema": "http://adaptivecards.io/schemas/adaptive-card.json"
                                }
                            }
                        }
                    }
                ]
            }

        }

    </script>

</head>

<body onload="renderCard()">
    <h1>Adaptive Cards Data Binding Example</h1>
    <div id="exampleDiv"></div>
</body>

</html>
```

## <a name="next-steps"></a><span data-ttu-id="4094f-125">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="4094f-125">Next steps</span></span>

- [<span data-ttu-id="4094f-126">Usar a API Pesquisa da Microsoft de usuário</span><span class="sxs-lookup"><span data-stu-id="4094f-126">Use the Microsoft Search API</span></span>](/graph/api/resources/search-api-overview)
