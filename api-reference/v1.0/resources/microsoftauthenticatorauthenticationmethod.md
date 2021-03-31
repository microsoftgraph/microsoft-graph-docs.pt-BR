---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethod
description: Uma representação do aplicativo Microsoft Authenticator registrado para um usuário. O Microsoft Authenticator é um método de autenticação.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f7438ca72a4f5d4063eec0444d3b0028237083d9
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468986"
---
# <a name="microsoftauthenticatorauthenticationmethod-resource-type"></a><span data-ttu-id="44ee4-104">Tipo de recurso microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="44ee4-104">microsoftAuthenticatorAuthenticationMethod resource type</span></span>

<span data-ttu-id="44ee4-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44ee4-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="44ee4-106">Uma representação do aplicativo Microsoft Authenticator registrado para um usuário.</span><span class="sxs-lookup"><span data-stu-id="44ee4-106">A representation of the Microsoft Authenticator app registered to a user.</span></span> <span data-ttu-id="44ee4-107">O Microsoft Authenticator é um método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="44ee4-107">Microsoft Authenticator is an authentication method.</span></span>

<span data-ttu-id="44ee4-108">Herda de [authenticationMethod](../resources/authenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="44ee4-108">Inherits from [authenticationMethod](../resources/authenticationmethod.md).</span></span>

## <a name="methods"></a><span data-ttu-id="44ee4-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="44ee4-109">Methods</span></span>
|<span data-ttu-id="44ee4-110">Método</span><span class="sxs-lookup"><span data-stu-id="44ee4-110">Method</span></span>|<span data-ttu-id="44ee4-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="44ee4-111">Return type</span></span>|<span data-ttu-id="44ee4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="44ee4-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="44ee4-113">Listar microsoftAuthenticatorAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="44ee4-113">List microsoftAuthenticatorAuthenticationMethods</span></span>](../api/microsoftauthenticatorauthenticationmethod-list.md)|<span data-ttu-id="44ee4-114">[coleção microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="44ee4-114">[microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) collection</span></span>|<span data-ttu-id="44ee4-115">Obter uma lista dos [objetos microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="44ee4-115">Get a list of the [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>|
|[<span data-ttu-id="44ee4-116">Obter microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="44ee4-116">Get microsoftAuthenticatorAuthenticationMethod</span></span>](../api/microsoftauthenticatorauthenticationmethod-get.md)|[<span data-ttu-id="44ee4-117">microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="44ee4-117">microsoftAuthenticatorAuthenticationMethod</span></span>](../resources/microsoftauthenticatorauthenticationmethod.md)|<span data-ttu-id="44ee4-118">Leia as propriedades e as relações de um [objeto microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="44ee4-118">Read the properties and relationships of a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>|
|[<span data-ttu-id="44ee4-119">Excluir microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="44ee4-119">Delete microsoftAuthenticatorAuthenticationMethod</span></span>](../api/microsoftauthenticatorauthenticationmethod-delete.md)|<span data-ttu-id="44ee4-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="44ee4-120">None</span></span>|<span data-ttu-id="44ee4-121">Exclui um [objeto microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="44ee4-121">Deletes a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="44ee4-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44ee4-122">Properties</span></span>
|<span data-ttu-id="44ee4-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44ee4-123">Property</span></span>|<span data-ttu-id="44ee4-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="44ee4-124">Type</span></span>|<span data-ttu-id="44ee4-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="44ee4-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44ee4-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44ee4-126">createdDateTime</span></span>|<span data-ttu-id="44ee4-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44ee4-127">DateTimeOffset</span></span>|<span data-ttu-id="44ee4-128">A data e a hora em que esse aplicativo foi registrado.</span><span class="sxs-lookup"><span data-stu-id="44ee4-128">The date and time that this app was registered.</span></span> <span data-ttu-id="44ee4-129">Essa propriedade será nula se o dispositivo não estiver registrado para Entrada de Telefone sem senha.</span><span class="sxs-lookup"><span data-stu-id="44ee4-129">This property is null if the device is not registered for passwordless Phone Sign-In.</span></span>|
|<span data-ttu-id="44ee4-130">displayName</span><span class="sxs-lookup"><span data-stu-id="44ee4-130">displayName</span></span>|<span data-ttu-id="44ee4-131">String</span><span class="sxs-lookup"><span data-stu-id="44ee4-131">String</span></span>|<span data-ttu-id="44ee4-132">O nome do dispositivo no qual esse aplicativo está registrado.</span><span class="sxs-lookup"><span data-stu-id="44ee4-132">The name of the device on which this app is registered.</span></span>|
|<span data-ttu-id="44ee4-133">id</span><span class="sxs-lookup"><span data-stu-id="44ee4-133">id</span></span>|<span data-ttu-id="44ee4-134">String</span><span class="sxs-lookup"><span data-stu-id="44ee4-134">String</span></span>|<span data-ttu-id="44ee4-135">Um identificador exclusivo para esse método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="44ee4-135">A unique identifier for this authentication method.</span></span> <span data-ttu-id="44ee4-136">Herdado da [autenticaçãoMethod](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="44ee4-136">Inherited from [authenticationMethod](../resources/authenticationmethod.md)</span></span>|
|<span data-ttu-id="44ee4-137">deviceTag</span><span class="sxs-lookup"><span data-stu-id="44ee4-137">deviceTag</span></span>|<span data-ttu-id="44ee4-138">String</span><span class="sxs-lookup"><span data-stu-id="44ee4-138">String</span></span>|<span data-ttu-id="44ee4-139">Marcas que contêm metadados de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44ee4-139">Tags containing app metadata.</span></span>|
|<span data-ttu-id="44ee4-140">phoneAppVersion</span><span class="sxs-lookup"><span data-stu-id="44ee4-140">phoneAppVersion</span></span>|<span data-ttu-id="44ee4-141">String</span><span class="sxs-lookup"><span data-stu-id="44ee4-141">String</span></span>|<span data-ttu-id="44ee4-142">Versão numérica dessa instância do aplicativo Authenticator.</span><span class="sxs-lookup"><span data-stu-id="44ee4-142">Numerical version of this instance of the Authenticator app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44ee4-143">Relações</span><span class="sxs-lookup"><span data-stu-id="44ee4-143">Relationships</span></span>
|<span data-ttu-id="44ee4-144">Relação</span><span class="sxs-lookup"><span data-stu-id="44ee4-144">Relationship</span></span>|<span data-ttu-id="44ee4-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="44ee4-145">Type</span></span>|<span data-ttu-id="44ee4-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="44ee4-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44ee4-147">device</span><span class="sxs-lookup"><span data-stu-id="44ee4-147">device</span></span>|[<span data-ttu-id="44ee4-148">device</span><span class="sxs-lookup"><span data-stu-id="44ee4-148">device</span></span>](../resources/device.md)|<span data-ttu-id="44ee4-149">O dispositivo registrado no qual o Microsoft Authenticator reside.</span><span class="sxs-lookup"><span data-stu-id="44ee4-149">The registered device on which Microsoft Authenticator resides.</span></span> <span data-ttu-id="44ee4-150">Essa propriedade será nula se o dispositivo não estiver registrado para Entrada de Telefone sem senha.</span><span class="sxs-lookup"><span data-stu-id="44ee4-150">This property is null if the device is not registered for passwordless Phone Sign-In.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44ee4-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44ee4-151">JSON representation</span></span>
<span data-ttu-id="44ee4-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="44ee4-152">The following is a JSON representation of the resource.</span></span>
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
