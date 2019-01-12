---
title: recurso de educationOneRosterApiDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando a API OneRoster é usada como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 681a3331aba7bc84ac80911c4be8076d104f8a58
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938143"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="b5c46-103">recurso de educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="b5c46-103">educationOneRosterApiDataProvider resource</span></span>

> <span data-ttu-id="b5c46-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b5c46-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5c46-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b5c46-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b5c46-106">Usado para configurar o perfil de sincronização de dados da escola quando a [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) é usado como a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="b5c46-106">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="b5c46-107">Derivado do [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="b5c46-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b5c46-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b5c46-108">Properties</span></span>

| <span data-ttu-id="b5c46-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5c46-109">Property</span></span> | <span data-ttu-id="b5c46-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5c46-110">Type</span></span> | <span data-ttu-id="b5c46-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5c46-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b5c46-112">**URL de conexão**</span><span class="sxs-lookup"><span data-stu-id="b5c46-112">**connectionUrl**</span></span> | <span data-ttu-id="b5c46-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5c46-113">String</span></span> | <span data-ttu-id="b5c46-114">A URL da conexão para a instância de OneRoster.</span><span class="sxs-lookup"><span data-stu-id="b5c46-114">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="b5c46-115">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="b5c46-115">**schoolsIds**</span></span> | <span data-ttu-id="b5c46-116">String collection</span><span class="sxs-lookup"><span data-stu-id="b5c46-116">String collection</span></span> |  <span data-ttu-id="b5c46-117">A lista de sourcedIds escola para sincronizar.</span><span class="sxs-lookup"><span data-stu-id="b5c46-117">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="b5c46-118">**providerName**</span><span class="sxs-lookup"><span data-stu-id="b5c46-118">**providerName**</span></span> | <span data-ttu-id="b5c46-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5c46-119">String</span></span> | <span data-ttu-id="b5c46-120">O nome do provedor de serviços de OneRoster conforme definido pela [especificação OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span><span class="sxs-lookup"><span data-stu-id="b5c46-120">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="b5c46-121">**connectionSettings**</span><span class="sxs-lookup"><span data-stu-id="b5c46-121">**connectionSettings**</span></span> | [<span data-ttu-id="b5c46-122">educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="b5c46-122">educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="b5c46-123">Configurações de Conexão para a instância de OneRoster.</span><span class="sxs-lookup"><span data-stu-id="b5c46-123">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="b5c46-124">Deve ser do tipo [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) ou [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="b5c46-124">Should be of type [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="b5c46-125">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="b5c46-125">**customizations**</span></span> | [<span data-ttu-id="b5c46-126">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="b5c46-126">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="b5c46-127">Personalização opcional a ser aplicado ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="b5c46-127">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5c46-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b5c46-128">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
