---
title: tipo de recurso educationSynchronizationConnectionSettings
description: 'Representa as configurações de conexão do provedor. Isso permite que o sistema saiba como se conectar às APIs do provedor. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c82d912b13ca68dcdccd5ace0232ed65f92cd879
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972482"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="df7a7-104">tipo de recurso educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="df7a7-104">educationSynchronizationConnectionSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df7a7-105">Representa as configurações de conexão do provedor.</span><span class="sxs-lookup"><span data-stu-id="df7a7-105">Represents the provider connection settings.</span></span> <span data-ttu-id="df7a7-106">Isso permite que o sistema saiba como se conectar às APIs do provedor.</span><span class="sxs-lookup"><span data-stu-id="df7a7-106">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="df7a7-107">**Observação:** Esse tipo complexo é abstrato.</span><span class="sxs-lookup"><span data-stu-id="df7a7-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="df7a7-108">Consulte os tipos específicos de configurações de conexão listadas.</span><span class="sxs-lookup"><span data-stu-id="df7a7-108">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="df7a7-109">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="df7a7-109">Derived types</span></span>
| <span data-ttu-id="df7a7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="df7a7-110">Type</span></span> | <span data-ttu-id="df7a7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="df7a7-111">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="df7a7-112">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="df7a7-112">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="df7a7-113">Use este tipo para fornecer configurações de conexão do OAuth1.</span><span class="sxs-lookup"><span data-stu-id="df7a7-113">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="df7a7-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="df7a7-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="df7a7-115">Use este tipo para fornecer as configurações de conexão de credenciais de cliente do OAuth2.</span><span class="sxs-lookup"><span data-stu-id="df7a7-115">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="df7a7-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df7a7-116">Properties</span></span>

| <span data-ttu-id="df7a7-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df7a7-117">Property</span></span> | <span data-ttu-id="df7a7-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="df7a7-118">Type</span></span> | <span data-ttu-id="df7a7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="df7a7-119">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="df7a7-120">**clientId**</span><span class="sxs-lookup"><span data-stu-id="df7a7-120">**clientId**</span></span> | <span data-ttu-id="df7a7-121">String</span><span class="sxs-lookup"><span data-stu-id="df7a7-121">String</span></span> |  <span data-ttu-id="df7a7-122">ID do cliente usada para se conectar ao provedor.</span><span class="sxs-lookup"><span data-stu-id="df7a7-122">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="df7a7-123">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="df7a7-123">**clientSecret**</span></span> | <span data-ttu-id="df7a7-124">String</span><span class="sxs-lookup"><span data-stu-id="df7a7-124">String</span></span> |  <span data-ttu-id="df7a7-125">Segredo do cliente para autenticar a conexão com o provedor.</span><span class="sxs-lookup"><span data-stu-id="df7a7-125">Client secret to authenticate the connection to the provider.</span></span> |
