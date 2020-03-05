---
title: tipo de recurso educationSynchronizationConnectionSettings
description: 'Representa as configurações de conexão do provedor. Isso permite que o sistema saiba como se conectar às APIs do provedor. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9d972aec91218dfc9606da4c8aa88e27b63167d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500566"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="8c6f2-104">tipo de recurso educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="8c6f2-104">educationSynchronizationConnectionSettings resource type</span></span>

<span data-ttu-id="8c6f2-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8c6f2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c6f2-106">Representa as configurações de conexão do provedor.</span><span class="sxs-lookup"><span data-stu-id="8c6f2-106">Represents the provider connection settings.</span></span> <span data-ttu-id="8c6f2-107">Isso permite que o sistema saiba como se conectar às APIs do provedor.</span><span class="sxs-lookup"><span data-stu-id="8c6f2-107">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="8c6f2-108">**Observação:** Esse tipo complexo é abstrato.</span><span class="sxs-lookup"><span data-stu-id="8c6f2-108">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="8c6f2-109">Consulte os tipos específicos de configurações de conexão listadas.</span><span class="sxs-lookup"><span data-stu-id="8c6f2-109">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="8c6f2-110">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="8c6f2-110">Derived types</span></span>
| <span data-ttu-id="8c6f2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c6f2-111">Type</span></span> | <span data-ttu-id="8c6f2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c6f2-112">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="8c6f2-113">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="8c6f2-113">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="8c6f2-114">Use este tipo para fornecer configurações de conexão do OAuth1.</span><span class="sxs-lookup"><span data-stu-id="8c6f2-114">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="8c6f2-115">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="8c6f2-115">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="8c6f2-116">Use este tipo para fornecer as configurações de conexão de credenciais de cliente do OAuth2.</span><span class="sxs-lookup"><span data-stu-id="8c6f2-116">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="8c6f2-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c6f2-117">Properties</span></span>

| <span data-ttu-id="8c6f2-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c6f2-118">Property</span></span> | <span data-ttu-id="8c6f2-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c6f2-119">Type</span></span> | <span data-ttu-id="8c6f2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c6f2-120">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="8c6f2-121">**clientId**</span><span class="sxs-lookup"><span data-stu-id="8c6f2-121">**clientId**</span></span> | <span data-ttu-id="8c6f2-122">String</span><span class="sxs-lookup"><span data-stu-id="8c6f2-122">String</span></span> |  <span data-ttu-id="8c6f2-123">ID do cliente usada para se conectar ao provedor.</span><span class="sxs-lookup"><span data-stu-id="8c6f2-123">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="8c6f2-124">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="8c6f2-124">**clientSecret**</span></span> | <span data-ttu-id="8c6f2-125">String</span><span class="sxs-lookup"><span data-stu-id="8c6f2-125">String</span></span> |  <span data-ttu-id="8c6f2-126">Segredo do cliente para autenticar a conexão com o provedor.</span><span class="sxs-lookup"><span data-stu-id="8c6f2-126">Client secret to authenticate the connection to the provider.</span></span> |
