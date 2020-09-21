---
title: recurso educationSynchronizationOAuth1ConnectionSettings
description: Quando o OAuth1 é usado para se conectar ao provedor de dados, esse tipo de configuração de conexão deve ser usado para configurar o perfil.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a73876185469ab762a08f409028880a4f7234d45
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989624"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a><span data-ttu-id="6944a-103">recurso educationSynchronizationOAuth1ConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="6944a-103">educationSynchronizationOAuth1ConnectionSettings resource</span></span>

<span data-ttu-id="6944a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6944a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6944a-105">Quando o OAuth1 é usado para se conectar ao provedor de dados, esse tipo de configuração de conexão deve ser usado para configurar o perfil.</span><span class="sxs-lookup"><span data-stu-id="6944a-105">When OAuth1 is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="6944a-106">Derivado de [educationSynchronizationConnectionSettings].</span><span class="sxs-lookup"><span data-stu-id="6944a-106">Derived from [educationSynchronizationConnectionSettings].</span></span>

## <a name="properties"></a><span data-ttu-id="6944a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6944a-107">Properties</span></span>

| <span data-ttu-id="6944a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6944a-108">Property</span></span>     | <span data-ttu-id="6944a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6944a-109">Type</span></span>   | <span data-ttu-id="6944a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6944a-110">Description</span></span>                                                                                                                |
| :----------- | :----- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6944a-111">clientId</span><span class="sxs-lookup"><span data-stu-id="6944a-111">clientId</span></span>     | <span data-ttu-id="6944a-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6944a-112">String</span></span> | <span data-ttu-id="6944a-113">ID do cliente usada para se conectar ao provedor.</span><span class="sxs-lookup"><span data-stu-id="6944a-113">Client ID used to connect to the provider.</span></span> <span data-ttu-id="6944a-114">Herdado de [educationSynchronizationConnectionSettings].</span><span class="sxs-lookup"><span data-stu-id="6944a-114">Inherited from [educationSynchronizationConnectionSettings].</span></span>                    |
| <span data-ttu-id="6944a-115">clientSecret</span><span class="sxs-lookup"><span data-stu-id="6944a-115">clientSecret</span></span> | <span data-ttu-id="6944a-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6944a-116">String</span></span> | <span data-ttu-id="6944a-117">Segredo do cliente para autenticar a conexão com o provedor.</span><span class="sxs-lookup"><span data-stu-id="6944a-117">Client secret to authenticate the connection to the provider.</span></span> <span data-ttu-id="6944a-118">Herdado de [educationSynchronizationConnectionSettings].</span><span class="sxs-lookup"><span data-stu-id="6944a-118">Inherited from [educationSynchronizationConnectionSettings].</span></span> |

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md

## <a name="json-representation"></a><span data-ttu-id="6944a-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6944a-120">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
  "clientId": "String",
  "clientSecret": "String"
}
```


