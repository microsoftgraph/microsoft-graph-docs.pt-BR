---
title: Tipo de recurso smsAuthenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação de Mensagem de Texto.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4309316adfeff126f845dd362d5ffb8899a77e60
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761027"
---
# <a name="smsauthenticationmethodtarget-resource-type"></a><span data-ttu-id="8c43c-103">Tipo de recurso smsAuthenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="8c43c-103">smsAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="8c43c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c43c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c43c-105">Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação de Mensagem [de](../resources/smsAuthenticationMethodConfiguration.md) Texto no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8c43c-105">A collection of users or groups enabled to use [Text Message authentication methods policy](../resources/smsAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="8c43c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c43c-106">Properties</span></span>
|<span data-ttu-id="8c43c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c43c-107">Property</span></span>|<span data-ttu-id="8c43c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c43c-108">Type</span></span>|<span data-ttu-id="8c43c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c43c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c43c-110">id</span><span class="sxs-lookup"><span data-stu-id="8c43c-110">id</span></span>|<span data-ttu-id="8c43c-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c43c-111">String</span></span>|<span data-ttu-id="8c43c-112">ID do objeto de um usuário ou grupo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8c43c-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="8c43c-113">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="8c43c-113">isRegistrationRequired</span></span>|<span data-ttu-id="8c43c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c43c-114">Boolean</span></span>|<span data-ttu-id="8c43c-115">Determina se o usuário é imposto a registrar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="8c43c-115">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="8c43c-116">**Não há suporte para**.</span><span class="sxs-lookup"><span data-stu-id="8c43c-116">**Not supported**.</span></span>|
|<span data-ttu-id="8c43c-117">isUsableForSignIn</span><span class="sxs-lookup"><span data-stu-id="8c43c-117">isUsableForSignIn</span></span>|<span data-ttu-id="8c43c-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c43c-118">Boolean</span></span>|<span data-ttu-id="8c43c-119">Determina se os usuários ou grupos podem usar esse método de autenticação para entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8c43c-119">Determines if the users or groups can use this authentication method to sign in to Azure AD.</span></span> <span data-ttu-id="8c43c-120">O valor é sempre `true` .</span><span class="sxs-lookup"><span data-stu-id="8c43c-120">The value is always `true`.</span></span>|
|<span data-ttu-id="8c43c-121">targetType</span><span class="sxs-lookup"><span data-stu-id="8c43c-121">targetType</span></span>|<span data-ttu-id="8c43c-122">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="8c43c-122">authenticationMethodTargetType</span></span>| <span data-ttu-id="8c43c-123">Os valores possíveis são: `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="8c43c-123">Possible values are: `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c43c-124">Relações</span><span class="sxs-lookup"><span data-stu-id="8c43c-124">Relationships</span></span>
<span data-ttu-id="8c43c-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8c43c-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c43c-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c43c-126">JSON representation</span></span>
<span data-ttu-id="8c43c-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c43c-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.smsAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodTarget",
  "targetType": "String",
  "id": "String (identifier)",
  "isRegistrationRequired": "Boolean",
  "isUsableForSignIn": "Boolean"
}
```
