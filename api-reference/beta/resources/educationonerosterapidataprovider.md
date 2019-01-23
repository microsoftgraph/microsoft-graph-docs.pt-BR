---
title: recurso de educationOneRosterApiDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando a API OneRoster é usada como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ccfb74cdac64a147adb8ed7d3a0ad4b3fa3c83cd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425985"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="ab36e-103">recurso de educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="ab36e-103">educationOneRosterApiDataProvider resource</span></span>

> <span data-ttu-id="ab36e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ab36e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab36e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ab36e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ab36e-106">Usado para configurar o perfil de sincronização de dados da escola quando a [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) é usado como a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="ab36e-106">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="ab36e-107">Derivado do [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="ab36e-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ab36e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab36e-108">Properties</span></span>

| <span data-ttu-id="ab36e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab36e-109">Property</span></span> | <span data-ttu-id="ab36e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab36e-110">Type</span></span> | <span data-ttu-id="ab36e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab36e-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="ab36e-112">**URL de conexão**</span><span class="sxs-lookup"><span data-stu-id="ab36e-112">**connectionUrl**</span></span> | <span data-ttu-id="ab36e-113">String</span><span class="sxs-lookup"><span data-stu-id="ab36e-113">String</span></span> | <span data-ttu-id="ab36e-114">A URL da conexão para a instância de OneRoster.</span><span class="sxs-lookup"><span data-stu-id="ab36e-114">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="ab36e-115">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="ab36e-115">**schoolsIds**</span></span> | <span data-ttu-id="ab36e-116">String collection</span><span class="sxs-lookup"><span data-stu-id="ab36e-116">String collection</span></span> |  <span data-ttu-id="ab36e-117">A lista de sourcedIds escola para sincronizar.</span><span class="sxs-lookup"><span data-stu-id="ab36e-117">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="ab36e-118">**providerName**</span><span class="sxs-lookup"><span data-stu-id="ab36e-118">**providerName**</span></span> | <span data-ttu-id="ab36e-119">String</span><span class="sxs-lookup"><span data-stu-id="ab36e-119">String</span></span> | <span data-ttu-id="ab36e-120">O nome do provedor de serviços de OneRoster conforme definido pela [especificação OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span><span class="sxs-lookup"><span data-stu-id="ab36e-120">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="ab36e-121">**connectionSettings**</span><span class="sxs-lookup"><span data-stu-id="ab36e-121">**connectionSettings**</span></span> | [<span data-ttu-id="ab36e-122">microsoft.graph.educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="ab36e-122">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="ab36e-123">Configurações de Conexão para a instância de OneRoster.</span><span class="sxs-lookup"><span data-stu-id="ab36e-123">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="ab36e-124">Deve ser do tipo [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) ou [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="ab36e-124">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="ab36e-125">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="ab36e-125">**customizations**</span></span> | [<span data-ttu-id="ab36e-126">microsoft.graph.educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="ab36e-126">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="ab36e-127">Personalização opcional a ser aplicado ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="ab36e-127">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab36e-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab36e-128">JSON representation</span></span>
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
