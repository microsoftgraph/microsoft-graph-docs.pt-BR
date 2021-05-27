---
title: tipo de recurso authenticationMethodsRegistrationCampaignIncludeTarget
description: Permitir que usuários e grupos de usuários sejam solicitados a configurar métodos de autenticação direcionada.
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 04dc753dd1a574bbf0b30d29b4b80375e7ab9a2c
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682862"
---
# <a name="authenticationmethodsregistrationcampaignincludetarget-resource-type"></a><span data-ttu-id="4ab2a-103">tipo de recurso authenticationMethodsRegistrationCampaignIncludeTarget</span><span class="sxs-lookup"><span data-stu-id="4ab2a-103">authenticationMethodsRegistrationCampaignIncludeTarget resource type</span></span>

<span data-ttu-id="4ab2a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ab2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ab2a-105">Representa os usuários e grupos direcionados para campanhas de registro do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-105">Represents the users and groups that are targeted for authentication method registration campaigns.</span></span> <span data-ttu-id="4ab2a-106">Somente usuários e grupos habilitados pela política para configurar o método de autenticação são direcionados.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-106">Only users and groups that are enabled by the policy to set up the authentication method are targeted.</span></span>

## <a name="properties"></a><span data-ttu-id="4ab2a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ab2a-107">Properties</span></span>
|<span data-ttu-id="4ab2a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ab2a-108">Property</span></span>|<span data-ttu-id="4ab2a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ab2a-109">Type</span></span>|<span data-ttu-id="4ab2a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ab2a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ab2a-111">id</span><span class="sxs-lookup"><span data-stu-id="4ab2a-111">id</span></span>|<span data-ttu-id="4ab2a-112">String</span><span class="sxs-lookup"><span data-stu-id="4ab2a-112">String</span></span>|<span data-ttu-id="4ab2a-113">O identificador de objeto de um usuário ou grupo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-113">The object identifier of an Azure AD user or group.</span></span>|
|<span data-ttu-id="4ab2a-114">targetedAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4ab2a-114">targetedAuthenticationMethod</span></span>|<span data-ttu-id="4ab2a-115">String</span><span class="sxs-lookup"><span data-stu-id="4ab2a-115">String</span></span>|<span data-ttu-id="4ab2a-116">O método de autenticação solicitado pelo usuário a registrar.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-116">The authentication method that the user is prompted to register.</span></span> <span data-ttu-id="4ab2a-117">O valor deve ser `microsoftAuthenticator` .</span><span class="sxs-lookup"><span data-stu-id="4ab2a-117">The value must be `microsoftAuthenticator`.</span></span>|
|<span data-ttu-id="4ab2a-118">targetType</span><span class="sxs-lookup"><span data-stu-id="4ab2a-118">targetType</span></span>|<span data-ttu-id="4ab2a-119">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="4ab2a-119">authenticationMethodTargetType</span></span>|<span data-ttu-id="4ab2a-120">O tipo de destino do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-120">The type of the authentication method target.</span></span> <span data-ttu-id="4ab2a-121">Os valores possíveis são: `user`, `group`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-121">Possible values are: `user`, `group`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ab2a-122">Relações</span><span class="sxs-lookup"><span data-stu-id="4ab2a-122">Relationships</span></span>
<span data-ttu-id="4ab2a-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ab2a-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ab2a-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ab2a-124">JSON representation</span></span>
<span data-ttu-id="4ab2a-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "targetedAuthenticationMethod": "String"
}
```
