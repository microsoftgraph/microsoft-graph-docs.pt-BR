---
title: recurso educationOneRosterApiDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando a API OneRoster é usada como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ca3341c84b79ff25e55be1abf5a8a5a031e84b02
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290382"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="11271-103">recurso educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="11271-103">educationOneRosterApiDataProvider resource</span></span>

<span data-ttu-id="11271-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11271-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11271-105">Usado para configurar o perfil de sincronização de dados da escola quando a [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) é usada como a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="11271-105">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="11271-106">Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="11271-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="11271-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11271-107">Properties</span></span>

| <span data-ttu-id="11271-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11271-108">Property</span></span> | <span data-ttu-id="11271-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="11271-109">Type</span></span> | <span data-ttu-id="11271-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="11271-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="11271-111">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="11271-111">**connectionUrl**</span></span> | <span data-ttu-id="11271-112">String</span><span class="sxs-lookup"><span data-stu-id="11271-112">String</span></span> | <span data-ttu-id="11271-113">A URL de conexão para a instância do OneRoster.</span><span class="sxs-lookup"><span data-stu-id="11271-113">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="11271-114">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="11271-114">**schoolsIds**</span></span> | <span data-ttu-id="11271-115">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="11271-115">String collection</span></span> |  <span data-ttu-id="11271-116">A lista de sourcedIds escolar a ser sincronizada.</span><span class="sxs-lookup"><span data-stu-id="11271-116">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="11271-117">**providerName**</span><span class="sxs-lookup"><span data-stu-id="11271-117">**providerName**</span></span> | <span data-ttu-id="11271-118">String</span><span class="sxs-lookup"><span data-stu-id="11271-118">String</span></span> | <span data-ttu-id="11271-119">O nome do provedor de serviços do OneRoster conforme definido pela [especificação OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span><span class="sxs-lookup"><span data-stu-id="11271-119">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="11271-120">**connectionSettings**</span><span class="sxs-lookup"><span data-stu-id="11271-120">**connectionSettings**</span></span> | [<span data-ttu-id="11271-121">Microsoft. Graph. educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="11271-121">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="11271-122">Configurações de conexão para a instância do OneRoster.</span><span class="sxs-lookup"><span data-stu-id="11271-122">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="11271-123">Deve ser do tipo [Microsoft. Graph. educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) ou [Microsoft. Graph. educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="11271-123">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="11271-124">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="11271-124">**customizations**</span></span> | [<span data-ttu-id="11271-125">Microsoft. Graph. educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="11271-125">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="11271-126">Personalização opcional a ser aplicada ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="11271-126">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11271-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11271-127">JSON representation</span></span>
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
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
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