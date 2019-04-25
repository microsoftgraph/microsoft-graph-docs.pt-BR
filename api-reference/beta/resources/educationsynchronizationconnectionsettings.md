---
title: tipo de recurso educationSynchronizationConnectionSettings
description: 'Representa as configurações de conexão do provedor. Isso permite que o sistema saiba como se conectar às APIs do provedor. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f6af6851e1e9d327b05c9ca1c7ed5929335a6e17
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542937"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="39e36-104">tipo de recurso educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="39e36-104">educationSynchronizationConnectionSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39e36-105">Representa as configurações de conexão do provedor.</span><span class="sxs-lookup"><span data-stu-id="39e36-105">Represents the provider connection settings.</span></span> <span data-ttu-id="39e36-106">Isso permite que o sistema saiba como se conectar às APIs do provedor.</span><span class="sxs-lookup"><span data-stu-id="39e36-106">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="39e36-107">**Observação:** Esse tipo complexo é abstrato.</span><span class="sxs-lookup"><span data-stu-id="39e36-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="39e36-108">Consulte os tipos específicos de configurações de conexão listadas.</span><span class="sxs-lookup"><span data-stu-id="39e36-108">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="39e36-109">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="39e36-109">Derived types</span></span>
| <span data-ttu-id="39e36-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="39e36-110">Type</span></span> | <span data-ttu-id="39e36-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="39e36-111">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="39e36-112">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="39e36-112">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="39e36-113">Use este tipo para fornecer configurações de conexão do OAuth1.</span><span class="sxs-lookup"><span data-stu-id="39e36-113">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="39e36-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="39e36-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="39e36-115">Use este tipo para fornecer as configurações de conexão de credenciais de cliente do OAuth2.</span><span class="sxs-lookup"><span data-stu-id="39e36-115">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="39e36-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="39e36-116">Properties</span></span>

| <span data-ttu-id="39e36-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39e36-117">Property</span></span> | <span data-ttu-id="39e36-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="39e36-118">Type</span></span> | <span data-ttu-id="39e36-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="39e36-119">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="39e36-120">**clientId**</span><span class="sxs-lookup"><span data-stu-id="39e36-120">**clientId**</span></span> | <span data-ttu-id="39e36-121">String</span><span class="sxs-lookup"><span data-stu-id="39e36-121">String</span></span> |  <span data-ttu-id="39e36-122">ID do cliente usada para se conectar ao provedor.</span><span class="sxs-lookup"><span data-stu-id="39e36-122">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="39e36-123">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="39e36-123">**clientSecret**</span></span> | <span data-ttu-id="39e36-124">String</span><span class="sxs-lookup"><span data-stu-id="39e36-124">String</span></span> |  <span data-ttu-id="39e36-125">Segredo do cliente para autenticar a conexão com o provedor.</span><span class="sxs-lookup"><span data-stu-id="39e36-125">Client secret to authenticate the connection to the provider.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationconnectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
