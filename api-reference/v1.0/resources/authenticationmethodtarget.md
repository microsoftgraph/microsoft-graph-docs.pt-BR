---
title: tipo de recurso authenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar um método de autenticação como parte de uma política de método de autenticação.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2f75a0ee81f1c43923a910bd86df4828c276706e
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469105"
---
# <a name="authenticationmethodtarget-resource-type"></a><span data-ttu-id="488f7-103">tipo de recurso authenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="488f7-103">authenticationMethodTarget resource type</span></span>

<span data-ttu-id="488f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="488f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="488f7-105">Uma coleção de usuários ou grupos habilitados para usar um método de autenticação como parte de uma política de método de autenticação no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="488f7-105">A collection of users or groups enabled to use an authentication method as part of an authentication method policy in Azure AD.</span></span>


## <a name="properties"></a><span data-ttu-id="488f7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="488f7-106">Properties</span></span>
|<span data-ttu-id="488f7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="488f7-107">Property</span></span>|<span data-ttu-id="488f7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="488f7-108">Type</span></span>|<span data-ttu-id="488f7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="488f7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="488f7-110">id</span><span class="sxs-lookup"><span data-stu-id="488f7-110">id</span></span>|<span data-ttu-id="488f7-111">String</span><span class="sxs-lookup"><span data-stu-id="488f7-111">String</span></span>|<span data-ttu-id="488f7-112">ID do objeto de um usuário ou grupo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="488f7-112">Object Id of an Azure AD user or group.</span></span>|
|<span data-ttu-id="488f7-113">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="488f7-113">isRegistrationRequired</span></span>|<span data-ttu-id="488f7-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="488f7-114">Boolean</span></span>|<span data-ttu-id="488f7-115">Determina se o usuário é imposto a registrar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="488f7-115">Determines if the user is enforced to register the authentication method.</span></span>|
|<span data-ttu-id="488f7-116">targetType</span><span class="sxs-lookup"><span data-stu-id="488f7-116">targetType</span></span>|<span data-ttu-id="488f7-117">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="488f7-117">authenticationMethodTargetType</span></span>|<span data-ttu-id="488f7-118">Os valores possíveis são: `user` e `group`.</span><span class="sxs-lookup"><span data-stu-id="488f7-118">Possible values are: `user`, `group`.</span></span>|
|<span data-ttu-id="488f7-119">useForSignIn</span><span class="sxs-lookup"><span data-stu-id="488f7-119">useForSignIn</span></span>|<span data-ttu-id="488f7-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="488f7-120">Boolean</span></span>|<span data-ttu-id="488f7-121">Determina se o método de autenticação pode ser usado para entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="488f7-121">Determines if the authentication method can be used to sign in to Azure AD.</span></span>|

## <a name="relationships"></a><span data-ttu-id="488f7-122">Relações</span><span class="sxs-lookup"><span data-stu-id="488f7-122">Relationships</span></span>
<span data-ttu-id="488f7-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="488f7-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="488f7-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="488f7-124">JSON representation</span></span>
<span data-ttu-id="488f7-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="488f7-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodTarget",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean"
}
```
