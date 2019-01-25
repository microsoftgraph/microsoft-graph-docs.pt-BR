---
title: recurso de educationOneRosterApiDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando a API OneRoster é usada como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 55a3cd0e20f15c4b7d44bc7aebdc19f202e044f1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527980"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="99418-103">recurso de educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="99418-103">educationOneRosterApiDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99418-104">Usado para configurar o perfil de sincronização de dados da escola quando a [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) é usado como a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="99418-104">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="99418-105">Derivado do [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="99418-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="99418-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99418-106">Properties</span></span>

| <span data-ttu-id="99418-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99418-107">Property</span></span> | <span data-ttu-id="99418-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="99418-108">Type</span></span> | <span data-ttu-id="99418-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="99418-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="99418-110">**URL de conexão**</span><span class="sxs-lookup"><span data-stu-id="99418-110">**connectionUrl**</span></span> | <span data-ttu-id="99418-111">String</span><span class="sxs-lookup"><span data-stu-id="99418-111">String</span></span> | <span data-ttu-id="99418-112">A URL da conexão para a instância de OneRoster.</span><span class="sxs-lookup"><span data-stu-id="99418-112">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="99418-113">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="99418-113">**schoolsIds**</span></span> | <span data-ttu-id="99418-114">String collection</span><span class="sxs-lookup"><span data-stu-id="99418-114">String collection</span></span> |  <span data-ttu-id="99418-115">A lista de sourcedIds escola para sincronizar.</span><span class="sxs-lookup"><span data-stu-id="99418-115">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="99418-116">ProviderName</span><span class="sxs-lookup"><span data-stu-id="99418-116">**providerName**</span></span> | <span data-ttu-id="99418-117">String</span><span class="sxs-lookup"><span data-stu-id="99418-117">String</span></span> | <span data-ttu-id="99418-118">O nome do provedor de serviços de OneRoster conforme definido pela [especificação OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span><span class="sxs-lookup"><span data-stu-id="99418-118">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="99418-119">**connectionSettings**</span><span class="sxs-lookup"><span data-stu-id="99418-119">**connectionSettings**</span></span> | [<span data-ttu-id="99418-120">microsoft.graph.educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="99418-120">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="99418-121">Configurações de Conexão para a instância de OneRoster.</span><span class="sxs-lookup"><span data-stu-id="99418-121">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="99418-122">Deve ser do tipo [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) ou [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="99418-122">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="99418-123">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="99418-123">**customizations**</span></span> | [<span data-ttu-id="99418-124">microsoft.graph.educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="99418-124">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="99418-125">Personalização opcional a ser aplicado ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="99418-125">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99418-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99418-126">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationonerosterapidataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
