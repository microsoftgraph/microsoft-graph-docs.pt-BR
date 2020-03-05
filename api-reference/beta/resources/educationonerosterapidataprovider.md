---
title: recurso educationOneRosterApiDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando a API OneRoster é usada como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 540a508ae3ac7d2b2ecf0f4cec2862b1331e4958
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501525"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="24232-103">recurso educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="24232-103">educationOneRosterApiDataProvider resource</span></span>

<span data-ttu-id="24232-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="24232-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24232-105">Usado para configurar o perfil de sincronização de dados da escola quando a [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) é usada como a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="24232-105">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="24232-106">Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="24232-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="24232-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="24232-107">Properties</span></span>

| <span data-ttu-id="24232-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24232-108">Property</span></span> | <span data-ttu-id="24232-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="24232-109">Type</span></span> | <span data-ttu-id="24232-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="24232-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="24232-111">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="24232-111">**connectionUrl**</span></span> | <span data-ttu-id="24232-112">String</span><span class="sxs-lookup"><span data-stu-id="24232-112">String</span></span> | <span data-ttu-id="24232-113">A URL de conexão para a instância do OneRoster.</span><span class="sxs-lookup"><span data-stu-id="24232-113">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="24232-114">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="24232-114">**schoolsIds**</span></span> | <span data-ttu-id="24232-115">String collection</span><span class="sxs-lookup"><span data-stu-id="24232-115">String collection</span></span> |  <span data-ttu-id="24232-116">A lista de sourcedIds escolar a ser sincronizada.</span><span class="sxs-lookup"><span data-stu-id="24232-116">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="24232-117">**providerName**</span><span class="sxs-lookup"><span data-stu-id="24232-117">**providerName**</span></span> | <span data-ttu-id="24232-118">String</span><span class="sxs-lookup"><span data-stu-id="24232-118">String</span></span> | <span data-ttu-id="24232-119">O nome do provedor de serviços do OneRoster conforme definido pela [especificação OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span><span class="sxs-lookup"><span data-stu-id="24232-119">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="24232-120">**connectionSettings**</span><span class="sxs-lookup"><span data-stu-id="24232-120">**connectionSettings**</span></span> | [<span data-ttu-id="24232-121">Microsoft. Graph. educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="24232-121">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="24232-122">Configurações de conexão para a instância do OneRoster.</span><span class="sxs-lookup"><span data-stu-id="24232-122">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="24232-123">Deve ser do tipo [Microsoft. Graph. educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) ou [Microsoft. Graph. educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="24232-123">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="24232-124">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="24232-124">**customizations**</span></span> | [<span data-ttu-id="24232-125">Microsoft. Graph. educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="24232-125">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="24232-126">Personalização opcional a ser aplicada ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="24232-126">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24232-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="24232-127">JSON representation</span></span>
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
