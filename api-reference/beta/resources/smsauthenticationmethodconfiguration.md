---
title: tipo de recurso smsAuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação de mensagem de texto.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c5a5e62e17e5b2e1cbc96ed96a44a0c483db981d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761034"
---
# <a name="smsauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="3d1b5-103">tipo de recurso smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="3d1b5-103">smsAuthenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="3d1b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d1b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d1b5-105">Representa uma política de métodos de autenticação de mensagem de texto.</span><span class="sxs-lookup"><span data-stu-id="3d1b5-105">Represents a Text Message authentication methods policy.</span></span> <span data-ttu-id="3d1b5-106">As políticas de métodos de autenticação definem configurações e usuários ou grupos habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3d1b5-106">Authentication methods policies define configuration settings and users or groups that are enabled to use the authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="3d1b5-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="3d1b5-107">Methods</span></span>
|<span data-ttu-id="3d1b5-108">Método</span><span class="sxs-lookup"><span data-stu-id="3d1b5-108">Method</span></span>|<span data-ttu-id="3d1b5-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3d1b5-109">Return type</span></span>|<span data-ttu-id="3d1b5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d1b5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3d1b5-111">Get</span><span class="sxs-lookup"><span data-stu-id="3d1b5-111">Get</span></span>](../api/smsauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="3d1b5-112">smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="3d1b5-112">smsAuthenticationMethodConfiguration</span></span>](../resources/smsauthenticationmethodconfiguration.md)|<span data-ttu-id="3d1b5-113">Leia as propriedades e as relações de um objeto smsAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3d1b5-113">Read the properties and relationships of a smsAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="3d1b5-114">Update</span><span class="sxs-lookup"><span data-stu-id="3d1b5-114">Update</span></span>](../api/smsauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="3d1b5-115">smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="3d1b5-115">smsAuthenticationMethodConfiguration</span></span>](../resources/smsauthenticationmethodconfiguration.md)|<span data-ttu-id="3d1b5-116">Atualize as propriedades de um objeto smsAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3d1b5-116">Update the properties of a smsAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="3d1b5-117">Delete</span><span class="sxs-lookup"><span data-stu-id="3d1b5-117">Delete</span></span>](../api/smsauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="3d1b5-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3d1b5-118">None</span></span>|<span data-ttu-id="3d1b5-119">Reverte o objeto smsAuthenticationMethodConfiguration para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="3d1b5-119">Reverts the smsAuthenticationMethodConfiguration object to its default configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="3d1b5-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d1b5-120">Properties</span></span>
|<span data-ttu-id="3d1b5-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d1b5-121">Property</span></span>|<span data-ttu-id="3d1b5-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d1b5-122">Type</span></span>|<span data-ttu-id="3d1b5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d1b5-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d1b5-124">id</span><span class="sxs-lookup"><span data-stu-id="3d1b5-124">id</span></span>|<span data-ttu-id="3d1b5-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d1b5-125">String</span></span>|<span data-ttu-id="3d1b5-126">O identificador de política do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3d1b5-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="3d1b5-127">state</span><span class="sxs-lookup"><span data-stu-id="3d1b5-127">state</span></span>|<span data-ttu-id="3d1b5-128">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="3d1b5-128">authenticationMethodState</span></span>|<span data-ttu-id="3d1b5-129">Os valores possíveis são: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="3d1b5-129">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d1b5-130">Relações</span><span class="sxs-lookup"><span data-stu-id="3d1b5-130">Relationships</span></span>
|<span data-ttu-id="3d1b5-131">Relação</span><span class="sxs-lookup"><span data-stu-id="3d1b5-131">Relationship</span></span>|<span data-ttu-id="3d1b5-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d1b5-132">Type</span></span>|<span data-ttu-id="3d1b5-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d1b5-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d1b5-134">includeTargets</span><span class="sxs-lookup"><span data-stu-id="3d1b5-134">includeTargets</span></span>|<span data-ttu-id="3d1b5-135">[coleção smsAuthenticationMethodTarget](../resources/smsauthenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="3d1b5-135">[smsAuthenticationMethodTarget](../resources/smsauthenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="3d1b5-136">Uma coleção de usuários ou grupos habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3d1b5-136">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d1b5-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d1b5-137">JSON representation</span></span>
<span data-ttu-id="3d1b5-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d1b5-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.smsAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```

