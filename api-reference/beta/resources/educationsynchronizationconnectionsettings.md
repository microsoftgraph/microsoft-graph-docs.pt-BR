---
title: tipo de recurso educationSynchronizationConnectionSettings
description: 'Representa as configurações de conexão do provedor. Isso permite que o sistema saiba como se conectar às APIs do provedor. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 387c002240d54d1ec12e58564e91831d6f0e8a50
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334099"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="22f9f-104">tipo de recurso educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="22f9f-104">educationSynchronizationConnectionSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22f9f-105">Representa as configurações de conexão do provedor.</span><span class="sxs-lookup"><span data-stu-id="22f9f-105">Represents the provider connection settings.</span></span> <span data-ttu-id="22f9f-106">Isso permite que o sistema saiba como se conectar às APIs do provedor.</span><span class="sxs-lookup"><span data-stu-id="22f9f-106">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="22f9f-107">**Observação:** Esse tipo complexo é abstrato.</span><span class="sxs-lookup"><span data-stu-id="22f9f-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="22f9f-108">Consulte os tipos específicos de configurações de conexão listadas.</span><span class="sxs-lookup"><span data-stu-id="22f9f-108">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="22f9f-109">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="22f9f-109">Derived types</span></span>
| <span data-ttu-id="22f9f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="22f9f-110">Type</span></span> | <span data-ttu-id="22f9f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="22f9f-111">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="22f9f-112">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="22f9f-112">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="22f9f-113">Use este tipo para fornecer configurações de conexão do OAuth1.</span><span class="sxs-lookup"><span data-stu-id="22f9f-113">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="22f9f-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="22f9f-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="22f9f-115">Use este tipo para fornecer as configurações de conexão de credenciais de cliente do OAuth2.</span><span class="sxs-lookup"><span data-stu-id="22f9f-115">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="22f9f-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22f9f-116">Properties</span></span>

| <span data-ttu-id="22f9f-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22f9f-117">Property</span></span> | <span data-ttu-id="22f9f-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="22f9f-118">Type</span></span> | <span data-ttu-id="22f9f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="22f9f-119">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="22f9f-120">**clientId**</span><span class="sxs-lookup"><span data-stu-id="22f9f-120">**clientId**</span></span> | <span data-ttu-id="22f9f-121">String</span><span class="sxs-lookup"><span data-stu-id="22f9f-121">String</span></span> |  <span data-ttu-id="22f9f-122">ID do cliente usada para se conectar ao provedor.</span><span class="sxs-lookup"><span data-stu-id="22f9f-122">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="22f9f-123">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="22f9f-123">**clientSecret**</span></span> | <span data-ttu-id="22f9f-124">String</span><span class="sxs-lookup"><span data-stu-id="22f9f-124">String</span></span> |  <span data-ttu-id="22f9f-125">Segredo do cliente para autenticar a conexão com o provedor.</span><span class="sxs-lookup"><span data-stu-id="22f9f-125">Client secret to authenticate the connection to the provider.</span></span> |
