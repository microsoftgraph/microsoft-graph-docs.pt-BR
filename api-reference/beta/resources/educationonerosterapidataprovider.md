---
title: recurso educationOneRosterApiDataProvider
description: Usado para configurar o perfil de sincronização de dados escolares quando a API do OneRoster é usada como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2c90c7132f6e51b84e987cf6bda63baacc60b8ba
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080418"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="7c69c-103">recurso educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="7c69c-103">educationOneRosterApiDataProvider resource</span></span>

<span data-ttu-id="7c69c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c69c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c69c-105">Usado para configurar o perfil de sincronização de dados escolares quando a [API do OneRoster](https://www.imsglobal.org/activity/onerosterlis) é usada como a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="7c69c-105">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="7c69c-106">Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="7c69c-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7c69c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c69c-107">Properties</span></span>

| <span data-ttu-id="7c69c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c69c-108">Property</span></span>           | <span data-ttu-id="7c69c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c69c-109">Type</span></span>                                         | <span data-ttu-id="7c69c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c69c-110">Description</span></span>                                                                                           |
| :----------------- | :------------------------------------------- | :---------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7c69c-111">connectionUrl</span><span class="sxs-lookup"><span data-stu-id="7c69c-111">connectionUrl</span></span>      | <span data-ttu-id="7c69c-112">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="7c69c-112">String</span></span>                                       | <span data-ttu-id="7c69c-113">A URL da conexão com a instância do OneRoster.</span><span class="sxs-lookup"><span data-stu-id="7c69c-113">The connection URL to the OneRoster instance.</span></span>                                                         |
| <span data-ttu-id="7c69c-114">providerName</span><span class="sxs-lookup"><span data-stu-id="7c69c-114">providerName</span></span>       | <span data-ttu-id="7c69c-115">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="7c69c-115">String</span></span>                                       | <span data-ttu-id="7c69c-116">O nome do Provedor de Serviços do OneRoster conforme definido pela [especificação do OneRoster][oneroster].</span><span class="sxs-lookup"><span data-stu-id="7c69c-116">The OneRoster Service Provider name as defined by the [OneRoster specification][oneroster].</span></span>           |
| <span data-ttu-id="7c69c-117">schoolsIds</span><span class="sxs-lookup"><span data-stu-id="7c69c-117">schoolsIds</span></span>         | <span data-ttu-id="7c69c-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c69c-118">String collection</span></span>                            | <span data-ttu-id="7c69c-119">A lista de [Escola/Organização a][orgs] `sourcedId` ser sincronizada.</span><span class="sxs-lookup"><span data-stu-id="7c69c-119">The list of [School/Org][orgs] `sourcedId` to sync.</span></span>                                                   |
| <span data-ttu-id="7c69c-120">termIds</span><span class="sxs-lookup"><span data-stu-id="7c69c-120">termIds</span></span>            | <span data-ttu-id="7c69c-121">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c69c-121">String collection</span></span>                            | <span data-ttu-id="7c69c-122">A lista de [sessões acadêmicas][terms] a sincronizar.</span><span class="sxs-lookup"><span data-stu-id="7c69c-122">The list of [academic sessions][terms] to sync.</span></span>                                                       |
| <span data-ttu-id="7c69c-123">connectionSettings</span><span class="sxs-lookup"><span data-stu-id="7c69c-123">connectionSettings</span></span> | <span data-ttu-id="7c69c-124">[educationSynchronizationConnectionSettings]</span><span class="sxs-lookup"><span data-stu-id="7c69c-124">[educationSynchronizationConnectionSettings]</span></span> | <span data-ttu-id="7c69c-125">As [configurações OAuth 1.0][onerosteroauth1] ou [OAuth 2.0][onerosteroauth2] para a instância do OneRoster.</span><span class="sxs-lookup"><span data-stu-id="7c69c-125">The [OAuth 1.0][onerosteroauth1] or [OAuth 2.0][onerosteroauth2] settings for the OneRoster instance.</span></span> |
| <span data-ttu-id="7c69c-126">personalizações</span><span class="sxs-lookup"><span data-stu-id="7c69c-126">customizations</span></span>     | <span data-ttu-id="7c69c-127">[educationSynchronizationCustomizations]</span><span class="sxs-lookup"><span data-stu-id="7c69c-127">[educationSynchronizationCustomizations]</span></span>    | <span data-ttu-id="7c69c-128">Personalização opcional a ser aplicada ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="7c69c-128">Optional customization to be applied to the synchronization profile.</span></span>                                  |

> [!IMPORTANT]
> <span data-ttu-id="7c69c-129">O OneRoster usa sessões acadêmicas em vez de um único ano escolar para segmentar seus dados.</span><span class="sxs-lookup"><span data-stu-id="7c69c-129">OneRoster uses academic sessions rather than a single school year to segment their data.</span></span> <span data-ttu-id="7c69c-130">Essa segmentação é abstraida dentro School Data Sync interface do usuário, mas não essa API.</span><span class="sxs-lookup"><span data-stu-id="7c69c-130">This segmentation is abstracted away within School Data Sync UI but not this API.</span></span> <span data-ttu-id="7c69c-131">Você precisará chamar o ponto de extremidade do OneRoster para obter a coleção de IDs de sessão acadêmica para preencher `/terms` a `termIds` coleção.</span><span class="sxs-lookup"><span data-stu-id="7c69c-131">You will need to call the OneRoster `/terms` endpoint to get the collection of academic session IDs in order to populate the `termIds` collection.</span></span>

[educationSynchronizationConnectionSettings]: educationsynchronizationconnectionsettings.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md
[oneroster]: https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA
[onerosteroauth2]: educationsynchronizationoauth2clientcredentialsconnectionsettings.md
[onerosteroauth1]: educationsynchronizationoauth1connectionsettings.md
[terms]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452034
[orgs]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452016

## <a name="json-representation"></a><span data-ttu-id="7c69c-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c69c-134">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type&quot;: &quot;microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
  "connectionUrl": "String",
  "providerName": "String",
  "schoolsIds": ["String"],
  "termIds": ["String"],
  "connectionSettings": {
    "@odata.type": "microsoft.graph.educationSynchronizationConnectionSettings",
    "clientId": "String",
    "clientSecret&quot;: &quot;String"
  },
  "customizations": {
    "@odata.type&quot;: &quot;microsoft.graph.educationSynchronizationCustomizations"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOneRosterApiDataProvider resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
      "Error: microsoft.graph.educationoneRosterApiDataProvider/connectionSettings:\r\n      Referenced type microsoft.graph.educationSynchronizationConnectionSettings is not defined in the doc set! Potential suggestion: microsoft.graph.ediscovery.settings"
  ]
}-->


