---
title: tipo de recurso de educationSynchronizationConnectionSettings
description: 'Representa as configurações de conexão do provedor. Isso permite que o sistema para saber como conectar ao provedor de APIs. '
ms.openlocfilehash: 27cdd377318d3294be9802b7cf28e940d0ada31c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037402"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="5d2fa-104">tipo de recurso de educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="5d2fa-104">educationSynchronizationConnectionSettings resource type</span></span>

> <span data-ttu-id="5d2fa-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5d2fa-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d2fa-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5d2fa-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5d2fa-107">Representa as configurações de conexão do provedor.</span><span class="sxs-lookup"><span data-stu-id="5d2fa-107">Represents the provider connection settings.</span></span> <span data-ttu-id="5d2fa-108">Isso permite que o sistema para saber como conectar ao provedor de APIs.</span><span class="sxs-lookup"><span data-stu-id="5d2fa-108">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="5d2fa-109">**Observação:** Este tipo complexo é abstrato.</span><span class="sxs-lookup"><span data-stu-id="5d2fa-109">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="5d2fa-110">Consulte os tipos específicos de configurações de conexão listados.</span><span class="sxs-lookup"><span data-stu-id="5d2fa-110">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="5d2fa-111">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="5d2fa-111">Derived types</span></span>
| <span data-ttu-id="5d2fa-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d2fa-112">Type</span></span> | <span data-ttu-id="5d2fa-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d2fa-113">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="5d2fa-114">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="5d2fa-114">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="5d2fa-115">Use este tipo para fornecer configurações de conexão OAuth1.</span><span class="sxs-lookup"><span data-stu-id="5d2fa-115">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="5d2fa-116">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="5d2fa-116">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="5d2fa-117">Use este tipo para fornecer configurações de conexão de concessão de credenciais do cliente OAuth2.</span><span class="sxs-lookup"><span data-stu-id="5d2fa-117">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="5d2fa-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5d2fa-118">Properties</span></span>

| <span data-ttu-id="5d2fa-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d2fa-119">Property</span></span> | <span data-ttu-id="5d2fa-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d2fa-120">Type</span></span> | <span data-ttu-id="5d2fa-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d2fa-121">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="5d2fa-122">**clientId**</span><span class="sxs-lookup"><span data-stu-id="5d2fa-122">**clientId**</span></span> | <span data-ttu-id="5d2fa-123">String</span><span class="sxs-lookup"><span data-stu-id="5d2fa-123">String</span></span> |  <span data-ttu-id="5d2fa-124">ID do cliente usada para conexão com o provedor.</span><span class="sxs-lookup"><span data-stu-id="5d2fa-124">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="5d2fa-125">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="5d2fa-125">**clientSecret**</span></span> | <span data-ttu-id="5d2fa-126">String</span><span class="sxs-lookup"><span data-stu-id="5d2fa-126">String</span></span> |  <span data-ttu-id="5d2fa-127">Segredo do cliente para autenticar a conexão ao provedor.</span><span class="sxs-lookup"><span data-stu-id="5d2fa-127">Client secret to authenticate the connection to the provider.</span></span> |