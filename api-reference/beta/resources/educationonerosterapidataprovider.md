---
title: recurso educationOneRosterApiDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando a API OneRoster é usada como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4ac232f71600f701efd8d085386fa9070773b475
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334181"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="fba19-103">recurso educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="fba19-103">educationOneRosterApiDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fba19-104">Usado para configurar o perfil de sincronização de dados da escola quando a [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) é usada como a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="fba19-104">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="fba19-105">Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="fba19-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fba19-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fba19-106">Properties</span></span>

| <span data-ttu-id="fba19-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fba19-107">Property</span></span> | <span data-ttu-id="fba19-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fba19-108">Type</span></span> | <span data-ttu-id="fba19-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fba19-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="fba19-110">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="fba19-110">**connectionUrl**</span></span> | <span data-ttu-id="fba19-111">String</span><span class="sxs-lookup"><span data-stu-id="fba19-111">String</span></span> | <span data-ttu-id="fba19-112">A URL de conexão para a instância do OneRoster.</span><span class="sxs-lookup"><span data-stu-id="fba19-112">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="fba19-113">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="fba19-113">**schoolsIds**</span></span> | <span data-ttu-id="fba19-114">Coleção String</span><span class="sxs-lookup"><span data-stu-id="fba19-114">String collection</span></span> |  <span data-ttu-id="fba19-115">A lista de sourcedIds escolar a ser sincronizada.</span><span class="sxs-lookup"><span data-stu-id="fba19-115">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="fba19-116">**providerName**</span><span class="sxs-lookup"><span data-stu-id="fba19-116">**providerName**</span></span> | <span data-ttu-id="fba19-117">String</span><span class="sxs-lookup"><span data-stu-id="fba19-117">String</span></span> | <span data-ttu-id="fba19-118">O nome do provedor de serviços do OneRoster conforme definido pela [especificação OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span><span class="sxs-lookup"><span data-stu-id="fba19-118">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="fba19-119">**connectionSettings**</span><span class="sxs-lookup"><span data-stu-id="fba19-119">**connectionSettings**</span></span> | [<span data-ttu-id="fba19-120">Microsoft. Graph. educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="fba19-120">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="fba19-121">Configurações de conexão para a instância do OneRoster.</span><span class="sxs-lookup"><span data-stu-id="fba19-121">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="fba19-122">Deve ser do tipo [Microsoft. Graph. educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) ou [Microsoft. Graph. educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="fba19-122">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="fba19-123">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="fba19-123">**customizations**</span></span> | [<span data-ttu-id="fba19-124">Microsoft. Graph. educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="fba19-124">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="fba19-125">Personalização opcional a ser aplicada ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="fba19-125">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fba19-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fba19-126">JSON representation</span></span>
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
