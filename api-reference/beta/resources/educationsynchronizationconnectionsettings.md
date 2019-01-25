---
title: tipo de recurso de educationSynchronizationConnectionSettings
description: 'Representa as configurações de conexão do provedor. Isso permite que o sistema para saber como conectar ao provedor de APIs. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f6af6851e1e9d327b05c9ca1c7ed5929335a6e17
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526862"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="8cbdf-104">tipo de recurso de educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="8cbdf-104">educationSynchronizationConnectionSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cbdf-105">Representa as configurações de conexão do provedor.</span><span class="sxs-lookup"><span data-stu-id="8cbdf-105">Represents the provider connection settings.</span></span> <span data-ttu-id="8cbdf-106">Isso permite que o sistema para saber como conectar ao provedor de APIs.</span><span class="sxs-lookup"><span data-stu-id="8cbdf-106">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="8cbdf-107">**Observação:** Este tipo complexo é abstrato.</span><span class="sxs-lookup"><span data-stu-id="8cbdf-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="8cbdf-108">Consulte os tipos específicos de configurações de conexão listados.</span><span class="sxs-lookup"><span data-stu-id="8cbdf-108">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="8cbdf-109">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="8cbdf-109">Derived types</span></span>
| <span data-ttu-id="8cbdf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cbdf-110">Type</span></span> | <span data-ttu-id="8cbdf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cbdf-111">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="8cbdf-112">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="8cbdf-112">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="8cbdf-113">Use este tipo para fornecer configurações de conexão OAuth1.</span><span class="sxs-lookup"><span data-stu-id="8cbdf-113">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="8cbdf-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="8cbdf-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="8cbdf-115">Use este tipo para fornecer configurações de conexão de concessão de credenciais do cliente OAuth2.</span><span class="sxs-lookup"><span data-stu-id="8cbdf-115">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="8cbdf-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8cbdf-116">Properties</span></span>

| <span data-ttu-id="8cbdf-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cbdf-117">Property</span></span> | <span data-ttu-id="8cbdf-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cbdf-118">Type</span></span> | <span data-ttu-id="8cbdf-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cbdf-119">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="8cbdf-120">**clientId**</span><span class="sxs-lookup"><span data-stu-id="8cbdf-120">**clientId**</span></span> | <span data-ttu-id="8cbdf-121">String</span><span class="sxs-lookup"><span data-stu-id="8cbdf-121">String</span></span> |  <span data-ttu-id="8cbdf-122">ID do cliente usada para conexão com o provedor.</span><span class="sxs-lookup"><span data-stu-id="8cbdf-122">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="8cbdf-123">client_secret</span><span class="sxs-lookup"><span data-stu-id="8cbdf-123">**clientSecret**</span></span> | <span data-ttu-id="8cbdf-124">String</span><span class="sxs-lookup"><span data-stu-id="8cbdf-124">String</span></span> |  <span data-ttu-id="8cbdf-125">Segredo do cliente para autenticar a conexão ao provedor.</span><span class="sxs-lookup"><span data-stu-id="8cbdf-125">Client secret to authenticate the connection to the provider.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationconnectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
