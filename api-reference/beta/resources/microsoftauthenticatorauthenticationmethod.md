---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethod
description: Uma representação do aplicativo Microsoft Authenticator registrado para um usuário. O Microsoft Authenticator é um método de autenticação.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f7438ca72a4f5d4063eec0444d3b0028237083d9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444137"
---
# <a name="microsoftauthenticatorauthenticationmethod-resource-type"></a><span data-ttu-id="c6472-104">Tipo de recurso microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c6472-104">microsoftAuthenticatorAuthenticationMethod resource type</span></span>

<span data-ttu-id="c6472-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6472-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c6472-106">Uma representação do aplicativo Microsoft Authenticator registrado para um usuário.</span><span class="sxs-lookup"><span data-stu-id="c6472-106">A representation of the Microsoft Authenticator app registered to a user.</span></span> <span data-ttu-id="c6472-107">O Microsoft Authenticator é um método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="c6472-107">Microsoft Authenticator is an authentication method.</span></span>

<span data-ttu-id="c6472-108">Herda de [authenticationMethod](../resources/authenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="c6472-108">Inherits from [authenticationMethod](../resources/authenticationmethod.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c6472-109">Methods</span><span class="sxs-lookup"><span data-stu-id="c6472-109">Methods</span></span>
|<span data-ttu-id="c6472-110">Método</span><span class="sxs-lookup"><span data-stu-id="c6472-110">Method</span></span>|<span data-ttu-id="c6472-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c6472-111">Return type</span></span>|<span data-ttu-id="c6472-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6472-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c6472-113">Listar microsoftAuthenticatorAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="c6472-113">List microsoftAuthenticatorAuthenticationMethods</span></span>](../api/microsoftauthenticatorauthenticationmethod-list.md)|<span data-ttu-id="c6472-114">[coleção microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="c6472-114">[microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) collection</span></span>|<span data-ttu-id="c6472-115">Obter uma lista dos [objetos microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="c6472-115">Get a list of the [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>|
|[<span data-ttu-id="c6472-116">Obter microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c6472-116">Get microsoftAuthenticatorAuthenticationMethod</span></span>](../api/microsoftauthenticatorauthenticationmethod-get.md)|[<span data-ttu-id="c6472-117">microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c6472-117">microsoftAuthenticatorAuthenticationMethod</span></span>](../resources/microsoftauthenticatorauthenticationmethod.md)|<span data-ttu-id="c6472-118">Leia as propriedades e as relações de um [objeto microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="c6472-118">Read the properties and relationships of a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>|
|[<span data-ttu-id="c6472-119">Excluir microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c6472-119">Delete microsoftAuthenticatorAuthenticationMethod</span></span>](../api/microsoftauthenticatorauthenticationmethod-delete.md)|<span data-ttu-id="c6472-120">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="c6472-120">None</span></span>|<span data-ttu-id="c6472-121">Exclui um [objeto microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="c6472-121">Deletes a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c6472-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6472-122">Properties</span></span>
|<span data-ttu-id="c6472-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6472-123">Property</span></span>|<span data-ttu-id="c6472-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6472-124">Type</span></span>|<span data-ttu-id="c6472-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6472-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6472-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6472-126">createdDateTime</span></span>|<span data-ttu-id="c6472-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6472-127">DateTimeOffset</span></span>|<span data-ttu-id="c6472-128">A data e a hora em que esse aplicativo foi registrado.</span><span class="sxs-lookup"><span data-stu-id="c6472-128">The date and time that this app was registered.</span></span> <span data-ttu-id="c6472-129">Essa propriedade será nula se o dispositivo não estiver registrado para Entrada de Telefone sem senha.</span><span class="sxs-lookup"><span data-stu-id="c6472-129">This property is null if the device is not registered for passwordless Phone Sign-In.</span></span>|
|<span data-ttu-id="c6472-130">displayName</span><span class="sxs-lookup"><span data-stu-id="c6472-130">displayName</span></span>|<span data-ttu-id="c6472-131">String</span><span class="sxs-lookup"><span data-stu-id="c6472-131">String</span></span>|<span data-ttu-id="c6472-132">O nome do dispositivo no qual esse aplicativo está registrado.</span><span class="sxs-lookup"><span data-stu-id="c6472-132">The name of the device on which this app is registered.</span></span>|
|<span data-ttu-id="c6472-133">id</span><span class="sxs-lookup"><span data-stu-id="c6472-133">id</span></span>|<span data-ttu-id="c6472-134">String</span><span class="sxs-lookup"><span data-stu-id="c6472-134">String</span></span>|<span data-ttu-id="c6472-135">Um identificador exclusivo para esse método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="c6472-135">A unique identifier for this authentication method.</span></span> <span data-ttu-id="c6472-136">Herdado da [autenticaçãoMethod](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="c6472-136">Inherited from [authenticationMethod](../resources/authenticationmethod.md)</span></span>|
|<span data-ttu-id="c6472-137">deviceTag</span><span class="sxs-lookup"><span data-stu-id="c6472-137">deviceTag</span></span>|<span data-ttu-id="c6472-138">String</span><span class="sxs-lookup"><span data-stu-id="c6472-138">String</span></span>|<span data-ttu-id="c6472-139">Marcas que contêm metadados de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c6472-139">Tags containing app metadata.</span></span>|
|<span data-ttu-id="c6472-140">phoneAppVersion</span><span class="sxs-lookup"><span data-stu-id="c6472-140">phoneAppVersion</span></span>|<span data-ttu-id="c6472-141">String</span><span class="sxs-lookup"><span data-stu-id="c6472-141">String</span></span>|<span data-ttu-id="c6472-142">Versão numérica dessa instância do aplicativo Authenticator.</span><span class="sxs-lookup"><span data-stu-id="c6472-142">Numerical version of this instance of the Authenticator app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6472-143">Relações</span><span class="sxs-lookup"><span data-stu-id="c6472-143">Relationships</span></span>
|<span data-ttu-id="c6472-144">Relação</span><span class="sxs-lookup"><span data-stu-id="c6472-144">Relationship</span></span>|<span data-ttu-id="c6472-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6472-145">Type</span></span>|<span data-ttu-id="c6472-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6472-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6472-147">device</span><span class="sxs-lookup"><span data-stu-id="c6472-147">device</span></span>|[<span data-ttu-id="c6472-148">device</span><span class="sxs-lookup"><span data-stu-id="c6472-148">device</span></span>](../resources/device.md)|<span data-ttu-id="c6472-149">O dispositivo registrado no qual o Microsoft Authenticator reside.</span><span class="sxs-lookup"><span data-stu-id="c6472-149">The registered device on which Microsoft Authenticator resides.</span></span> <span data-ttu-id="c6472-150">Essa propriedade será nula se o dispositivo não estiver registrado para Entrada de Telefone sem senha.</span><span class="sxs-lookup"><span data-stu-id="c6472-150">This property is null if the device is not registered for passwordless Phone Sign-In.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6472-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6472-151">JSON representation</span></span>
<span data-ttu-id="c6472-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c6472-152">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
  "id": "String (Identifier)",
  "displayName": "String",
  "deviceTag": "String",
  "phoneAppVersion": "String",
  "createdDateTime": "DateTimeOffset"
}
```
