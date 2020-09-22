---
title: recurso educationOneRosterApiDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando a API OneRoster é usada como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5b96322cdb408069136a46aa9c83cf363cc1b6f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998842"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="f0cbb-103">recurso educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="f0cbb-103">educationOneRosterApiDataProvider resource</span></span>

<span data-ttu-id="f0cbb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0cbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0cbb-105">Usado para configurar o perfil de sincronização de dados da escola quando a [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) é usada como a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="f0cbb-105">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="f0cbb-106">Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="f0cbb-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f0cbb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0cbb-107">Properties</span></span>

| <span data-ttu-id="f0cbb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0cbb-108">Property</span></span>           | <span data-ttu-id="f0cbb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0cbb-109">Type</span></span>                                         | <span data-ttu-id="f0cbb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0cbb-110">Description</span></span>                                                                                           |
| :----------------- | :------------------------------------------- | :---------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f0cbb-111">connectionUrl</span><span class="sxs-lookup"><span data-stu-id="f0cbb-111">connectionUrl</span></span>      | <span data-ttu-id="f0cbb-112">String</span><span class="sxs-lookup"><span data-stu-id="f0cbb-112">String</span></span>                                       | <span data-ttu-id="f0cbb-113">A URL de conexão para a instância do OneRoster.</span><span class="sxs-lookup"><span data-stu-id="f0cbb-113">The connection URL to the OneRoster instance.</span></span>                                                         |
| <span data-ttu-id="f0cbb-114">providerName</span><span class="sxs-lookup"><span data-stu-id="f0cbb-114">providerName</span></span>       | <span data-ttu-id="f0cbb-115">String</span><span class="sxs-lookup"><span data-stu-id="f0cbb-115">String</span></span>                                       | <span data-ttu-id="f0cbb-116">O nome do provedor de serviços do OneRoster conforme definido pela [especificação OneRoster][oneroster].</span><span class="sxs-lookup"><span data-stu-id="f0cbb-116">The OneRoster Service Provider name as defined by the [OneRoster specification][oneroster].</span></span>           |
| <span data-ttu-id="f0cbb-117">schoolsIds</span><span class="sxs-lookup"><span data-stu-id="f0cbb-117">schoolsIds</span></span>         | <span data-ttu-id="f0cbb-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0cbb-118">String collection</span></span>                            | <span data-ttu-id="f0cbb-119">A lista de [escolas/org][orgs] `sourcedId` a ser sincronizada.</span><span class="sxs-lookup"><span data-stu-id="f0cbb-119">The list of [School/Org][orgs] `sourcedId` to sync.</span></span>                                                   |
| <span data-ttu-id="f0cbb-120">termIds</span><span class="sxs-lookup"><span data-stu-id="f0cbb-120">termIds</span></span>            | <span data-ttu-id="f0cbb-121">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0cbb-121">String collection</span></span>                            | <span data-ttu-id="f0cbb-122">A lista de [sessões acadêmicas][terms] a serem sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="f0cbb-122">The list of [academic sessions][terms] to sync.</span></span>                                                       |
| <span data-ttu-id="f0cbb-123">connectionSettings</span><span class="sxs-lookup"><span data-stu-id="f0cbb-123">connectionSettings</span></span> | <span data-ttu-id="f0cbb-124">[educationSynchronizationConnectionSettings]</span><span class="sxs-lookup"><span data-stu-id="f0cbb-124">[educationSynchronizationConnectionSettings]</span></span> | <span data-ttu-id="f0cbb-125">As configurações do [oauth 1,0][onerosteroauth1] ou [OAuth 2,0][onerosteroauth2] para a instância do OneRoster.</span><span class="sxs-lookup"><span data-stu-id="f0cbb-125">The [OAuth 1.0][onerosteroauth1] or [OAuth 2.0][onerosteroauth2] settings for the OneRoster instance.</span></span> |
| <span data-ttu-id="f0cbb-126">personalizações</span><span class="sxs-lookup"><span data-stu-id="f0cbb-126">customizations</span></span>     | <span data-ttu-id="f0cbb-127">[educationSynchronizationCustomizations])</span><span class="sxs-lookup"><span data-stu-id="f0cbb-127">[educationSynchronizationCustomizations])</span></span>    | <span data-ttu-id="f0cbb-128">Personalização opcional a ser aplicada ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="f0cbb-128">Optional customization to be applied to the synchronization profile.</span></span>                                  |

> [!IMPORTANT]
> <span data-ttu-id="f0cbb-129">O OneRoster usa sessões acadêmicas em vez de um único ano escolar para segmentar seus dados.</span><span class="sxs-lookup"><span data-stu-id="f0cbb-129">OneRoster uses academic sessions rather than a single school year to segment their data.</span></span> <span data-ttu-id="f0cbb-130">Essa segmentação é dissociada na interface de usuário de sincronização de dados da escola, mas não esta API.</span><span class="sxs-lookup"><span data-stu-id="f0cbb-130">This segmentation is abstracted away within School Data Sync UI but not this API.</span></span> <span data-ttu-id="f0cbb-131">Você precisará chamar o ponto de `/terms` extremidade do OneRoster para obter a coleção de IDs de sessão acadêmica a fim de preencher a `termIds` coleção.</span><span class="sxs-lookup"><span data-stu-id="f0cbb-131">You will need to call the OneRoster `/terms` endpoint to get the collection of academic session IDs in order to populate the `termIds` collection.</span></span>

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md
[oneroster]: https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA
[onerosteroauth2]: educationsynchronizationoauth2clientcredentialsconnectionsettings.md
[onerosteroauth1]: educationsynchronizationoauth1connectionsettings.md
[terms]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452034
[orgs]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452016

## <a name="json-representation"></a><span data-ttu-id="f0cbb-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0cbb-134">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
  "connectionUrl": "String",
  "providerName": "String",
  "schoolsIds": ["String"],
  "termIds": ["String"],
  "connectionSettings": {
    "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
  },
  "customizations": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
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
      "Error: microsoft.graph.educationoneRosterApiDataProvider/connectionSettings:\r\n      Referenced type microsoft.graph.educationSynchronizationConnectionSettings is not defined in the doc set! Potential suggestion: microsoft.graph.settings"
  ]
}-->


