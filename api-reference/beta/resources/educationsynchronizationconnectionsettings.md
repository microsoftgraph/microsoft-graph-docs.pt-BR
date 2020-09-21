---
title: tipo de recurso educationSynchronizationConnectionSettings
description: 'Representa as configurações de conexão do provedor. Isso permite que o sistema saiba como se conectar às APIs do provedor. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 449dc1c4265355d55e6d3ceb51fe86be9f84ac31
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979557"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="94e81-104">tipo de recurso educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="94e81-104">educationSynchronizationConnectionSettings resource type</span></span>

<span data-ttu-id="94e81-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94e81-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94e81-106">Representa as configurações de conexão do provedor.</span><span class="sxs-lookup"><span data-stu-id="94e81-106">Represents the provider connection settings.</span></span> <span data-ttu-id="94e81-107">Isso permite que o sistema saiba como se conectar às APIs do provedor.</span><span class="sxs-lookup"><span data-stu-id="94e81-107">This allows the system to know how to connect to the provider APIs.</span></span>

> [!NOTE]
> <span data-ttu-id="94e81-108">Esse tipo complexo é abstrato.</span><span class="sxs-lookup"><span data-stu-id="94e81-108">This complex type is abstract.</span></span> <span data-ttu-id="94e81-109">Consulte os tipos específicos de configurações de conexão listadas.</span><span class="sxs-lookup"><span data-stu-id="94e81-109">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="94e81-110">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="94e81-110">Derived types</span></span>

| <span data-ttu-id="94e81-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="94e81-111">Type</span></span>                                                                                                                                      | <span data-ttu-id="94e81-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="94e81-112">Description</span></span>                                                                   |
| :---------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------- |
| [<span data-ttu-id="94e81-113">educationSynchronizationOAuth1ConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="94e81-113">educationSynchronizationOAuth1ConnectionSettings</span></span>](educationsynchronizationoauth1connectionsettings.md)                                   | <span data-ttu-id="94e81-114">Use este tipo para fornecer configurações de conexão do OAuth1.</span><span class="sxs-lookup"><span data-stu-id="94e81-114">Use this type to provide OAuth1 connection settings.</span></span>                          |
| [<span data-ttu-id="94e81-115">educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="94e81-115">educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="94e81-116">Use este tipo para fornecer as configurações de conexão de credenciais de cliente do OAuth2.</span><span class="sxs-lookup"><span data-stu-id="94e81-116">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="94e81-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94e81-117">Properties</span></span>

| <span data-ttu-id="94e81-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94e81-118">Property</span></span>     | <span data-ttu-id="94e81-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="94e81-119">Type</span></span>   | <span data-ttu-id="94e81-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="94e81-120">Description</span></span>                                                   |
| :----------- | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="94e81-121">clientId</span><span class="sxs-lookup"><span data-stu-id="94e81-121">clientId</span></span>     | <span data-ttu-id="94e81-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94e81-122">String</span></span> | <span data-ttu-id="94e81-123">ID do cliente usada para se conectar ao provedor.</span><span class="sxs-lookup"><span data-stu-id="94e81-123">Client ID used to connect to the provider.</span></span>                    |
| <span data-ttu-id="94e81-124">clientSecret</span><span class="sxs-lookup"><span data-stu-id="94e81-124">clientSecret</span></span> | <span data-ttu-id="94e81-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94e81-125">String</span></span> | <span data-ttu-id="94e81-126">Segredo do cliente para autenticar a conexão com o provedor.</span><span class="sxs-lookup"><span data-stu-id="94e81-126">Client secret to authenticate the connection to the provider.</span></span> |


