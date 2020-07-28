---
title: tipo de recurso educationSynchronizationConnectionSettings
description: 'Representa as configurações de conexão do provedor. Isso permite que o sistema saiba como se conectar às APIs do provedor. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 71da1acbd9910757375acbc22dda63f412f459b2
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434876"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="aa944-104">tipo de recurso educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="aa944-104">educationSynchronizationConnectionSettings resource type</span></span>

<span data-ttu-id="aa944-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa944-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa944-106">Representa as configurações de conexão do provedor.</span><span class="sxs-lookup"><span data-stu-id="aa944-106">Represents the provider connection settings.</span></span> <span data-ttu-id="aa944-107">Isso permite que o sistema saiba como se conectar às APIs do provedor.</span><span class="sxs-lookup"><span data-stu-id="aa944-107">This allows the system to know how to connect to the provider APIs.</span></span>

> [!NOTE]
> <span data-ttu-id="aa944-108">Esse tipo complexo é abstrato.</span><span class="sxs-lookup"><span data-stu-id="aa944-108">This complex type is abstract.</span></span> <span data-ttu-id="aa944-109">Consulte os tipos específicos de configurações de conexão listadas.</span><span class="sxs-lookup"><span data-stu-id="aa944-109">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="aa944-110">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="aa944-110">Derived types</span></span>

| <span data-ttu-id="aa944-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa944-111">Type</span></span>                                                                                                                                      | <span data-ttu-id="aa944-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa944-112">Description</span></span>                                                                   |
| :---------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------- |
| [<span data-ttu-id="aa944-113">educationSynchronizationOAuth1ConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="aa944-113">educationSynchronizationOAuth1ConnectionSettings</span></span>](educationsynchronizationoauth1connectionsettings.md)                                   | <span data-ttu-id="aa944-114">Use este tipo para fornecer configurações de conexão do OAuth1.</span><span class="sxs-lookup"><span data-stu-id="aa944-114">Use this type to provide OAuth1 connection settings.</span></span>                          |
| [<span data-ttu-id="aa944-115">educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="aa944-115">educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="aa944-116">Use este tipo para fornecer as configurações de conexão de credenciais de cliente do OAuth2.</span><span class="sxs-lookup"><span data-stu-id="aa944-116">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="aa944-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aa944-117">Properties</span></span>

| <span data-ttu-id="aa944-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa944-118">Property</span></span>     | <span data-ttu-id="aa944-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa944-119">Type</span></span>   | <span data-ttu-id="aa944-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa944-120">Description</span></span>                                                   |
| :----------- | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="aa944-121">clientId</span><span class="sxs-lookup"><span data-stu-id="aa944-121">clientId</span></span>     | <span data-ttu-id="aa944-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa944-122">String</span></span> | <span data-ttu-id="aa944-123">ID do cliente usada para se conectar ao provedor.</span><span class="sxs-lookup"><span data-stu-id="aa944-123">Client ID used to connect to the provider.</span></span>                    |
| <span data-ttu-id="aa944-124">clientSecret</span><span class="sxs-lookup"><span data-stu-id="aa944-124">clientSecret</span></span> | <span data-ttu-id="aa944-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa944-125">String</span></span> | <span data-ttu-id="aa944-126">Segredo do cliente para autenticar a conexão com o provedor.</span><span class="sxs-lookup"><span data-stu-id="aa944-126">Client secret to authenticate the connection to the provider.</span></span> |
