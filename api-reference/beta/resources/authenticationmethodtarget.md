---
title: tipo de recurso authenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar um método de autenticação como parte de uma política de método de autenticação.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7112249f618bbda31eddeb07967d201c8b641075
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418194"
---
# <a name="authenticationmethodtarget-resource-type"></a><span data-ttu-id="14cdb-103">tipo de recurso authenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="14cdb-103">authenticationMethodTarget resource type</span></span>

<span data-ttu-id="14cdb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14cdb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14cdb-105">Uma coleção de usuários ou grupos habilitados para usar um método de autenticação como parte de uma política de método de autenticação no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="14cdb-105">A collection of users or groups enabled to use an authentication method as part of an authentication method policy in Azure AD.</span></span>


## <a name="properties"></a><span data-ttu-id="14cdb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14cdb-106">Properties</span></span>
|<span data-ttu-id="14cdb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14cdb-107">Property</span></span>|<span data-ttu-id="14cdb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="14cdb-108">Type</span></span>|<span data-ttu-id="14cdb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="14cdb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14cdb-110">id</span><span class="sxs-lookup"><span data-stu-id="14cdb-110">id</span></span>|<span data-ttu-id="14cdb-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14cdb-111">String</span></span>|<span data-ttu-id="14cdb-112">ID de objeto de um usuário ou grupo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="14cdb-112">Object Id of an Azure AD user or group.</span></span>|
|<span data-ttu-id="14cdb-113">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="14cdb-113">isRegistrationRequired</span></span>|<span data-ttu-id="14cdb-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="14cdb-114">Boolean</span></span>|<span data-ttu-id="14cdb-115">Determina se o usuário é imposto para registrar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="14cdb-115">Determines if the user is enforced to register the authentication method.</span></span>|
|<span data-ttu-id="14cdb-116">targetType</span><span class="sxs-lookup"><span data-stu-id="14cdb-116">targetType</span></span>|<span data-ttu-id="14cdb-117">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="14cdb-117">authenticationMethodTargetType</span></span>|<span data-ttu-id="14cdb-118">Os valores possíveis são: `user` e `group`.</span><span class="sxs-lookup"><span data-stu-id="14cdb-118">Possible values are: `user`, `group`.</span></span>|
|<span data-ttu-id="14cdb-119">useForSignIn</span><span class="sxs-lookup"><span data-stu-id="14cdb-119">useForSignIn</span></span>|<span data-ttu-id="14cdb-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="14cdb-120">Boolean</span></span>|<span data-ttu-id="14cdb-121">Determina se o método de autenticação pode ser usado para entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="14cdb-121">Determines if the authentication method can be used to sign in to Azure AD.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14cdb-122">Relações</span><span class="sxs-lookup"><span data-stu-id="14cdb-122">Relationships</span></span>
<span data-ttu-id="14cdb-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="14cdb-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="14cdb-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14cdb-124">JSON representation</span></span>
<span data-ttu-id="14cdb-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="14cdb-125">The following is a JSON representation of the resource.</span></span>
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
