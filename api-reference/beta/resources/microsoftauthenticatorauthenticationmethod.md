---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethod
description: Uma representação do aplicativo Microsoft Authenticator registrado a um usuário. O Microsoft Authenticator é um método de autenticação.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aeb2d1d7b111c9424da2f927dbaf3030a356c6b6
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796715"
---
# <a name="microsoftauthenticatorauthenticationmethod-resource-type"></a><span data-ttu-id="b76ef-104">Tipo de recurso microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b76ef-104">microsoftAuthenticatorAuthenticationMethod resource type</span></span>

<span data-ttu-id="b76ef-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b76ef-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b76ef-106">Uma representação do aplicativo Microsoft Authenticator registrado a um usuário.</span><span class="sxs-lookup"><span data-stu-id="b76ef-106">A representation of the Microsoft Authenticator app registered to a user.</span></span> <span data-ttu-id="b76ef-107">O Microsoft Authenticator é um método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="b76ef-107">Microsoft Authenticator is an authentication method.</span></span>

<span data-ttu-id="b76ef-108">Herda de [authenticationMethod](../resources/authenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="b76ef-108">Inherits from [authenticationMethod](../resources/authenticationmethod.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b76ef-109">Methods</span><span class="sxs-lookup"><span data-stu-id="b76ef-109">Methods</span></span>
|<span data-ttu-id="b76ef-110">Método</span><span class="sxs-lookup"><span data-stu-id="b76ef-110">Method</span></span>|<span data-ttu-id="b76ef-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b76ef-111">Return type</span></span>|<span data-ttu-id="b76ef-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b76ef-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b76ef-113">Listar microsoftAuthenticatorAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="b76ef-113">List microsoftAuthenticatorAuthenticationMethods</span></span>](../api/microsoftauthenticatorauthenticationmethod-list.md)|<span data-ttu-id="b76ef-114">[Coleção microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="b76ef-114">[microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) collection</span></span>|<span data-ttu-id="b76ef-115">Obter uma lista dos [objetos microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="b76ef-115">Get a list of the [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>|
|[<span data-ttu-id="b76ef-116">Obter microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b76ef-116">Get microsoftAuthenticatorAuthenticationMethod</span></span>](../api/microsoftauthenticatorauthenticationmethod-get.md)|[<span data-ttu-id="b76ef-117">microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b76ef-117">microsoftAuthenticatorAuthenticationMethod</span></span>](../resources/microsoftauthenticatorauthenticationmethod.md)|<span data-ttu-id="b76ef-118">Leia as propriedades e os relacionamentos de um [objeto microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="b76ef-118">Read the properties and relationships of a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>|
|[<span data-ttu-id="b76ef-119">Excluir microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b76ef-119">Delete microsoftAuthenticatorAuthenticationMethod</span></span>](../api/microsoftauthenticatorauthenticationmethod-delete.md)|<span data-ttu-id="b76ef-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b76ef-120">None</span></span>|<span data-ttu-id="b76ef-121">Exclui um [objeto microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="b76ef-121">Deletes a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b76ef-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b76ef-122">Properties</span></span>
|<span data-ttu-id="b76ef-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b76ef-123">Property</span></span>|<span data-ttu-id="b76ef-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b76ef-124">Type</span></span>|<span data-ttu-id="b76ef-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b76ef-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b76ef-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b76ef-126">createdDateTime</span></span>|<span data-ttu-id="b76ef-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b76ef-127">DateTimeOffset</span></span>|<span data-ttu-id="b76ef-128">A data e a hora em que esse aplicativo foi registrado.</span><span class="sxs-lookup"><span data-stu-id="b76ef-128">The date and time that this app was registered.</span></span> <span data-ttu-id="b76ef-129">Essa propriedade será nula se o dispositivo não estiver registrado para entrada por telefone sem senha.</span><span class="sxs-lookup"><span data-stu-id="b76ef-129">This property is null if the device is not registered for passwordless Phone Sign-In.</span></span>|
|<span data-ttu-id="b76ef-130">displayName</span><span class="sxs-lookup"><span data-stu-id="b76ef-130">displayName</span></span>|<span data-ttu-id="b76ef-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b76ef-131">String</span></span>|<span data-ttu-id="b76ef-132">O nome do dispositivo no qual esse aplicativo está registrado.</span><span class="sxs-lookup"><span data-stu-id="b76ef-132">The name of the device on which this app is registered.</span></span>|
|<span data-ttu-id="b76ef-133">id</span><span class="sxs-lookup"><span data-stu-id="b76ef-133">id</span></span>|<span data-ttu-id="b76ef-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b76ef-134">String</span></span>|<span data-ttu-id="b76ef-135">Um identificador exclusivo para esse método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="b76ef-135">A unique identifier for this authentication method.</span></span> <span data-ttu-id="b76ef-136">Herdado de [authenticationMethod](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="b76ef-136">Inherited from [authenticationMethod](../resources/authenticationmethod.md)</span></span>|
|<span data-ttu-id="b76ef-137">deviceTag</span><span class="sxs-lookup"><span data-stu-id="b76ef-137">deviceTag</span></span>|<span data-ttu-id="b76ef-138">String</span><span class="sxs-lookup"><span data-stu-id="b76ef-138">String</span></span>|<span data-ttu-id="b76ef-139">Marcas que contêm metadados do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b76ef-139">Tags containing app metadata.</span></span>|
|<span data-ttu-id="b76ef-140">phoneAppVersion</span><span class="sxs-lookup"><span data-stu-id="b76ef-140">phoneAppVersion</span></span>|<span data-ttu-id="b76ef-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b76ef-141">String</span></span>|<span data-ttu-id="b76ef-142">Versão numérica desta instância do aplicativo Autenticador.</span><span class="sxs-lookup"><span data-stu-id="b76ef-142">Numerical version of this instance of the Authenticator app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b76ef-143">Relações</span><span class="sxs-lookup"><span data-stu-id="b76ef-143">Relationships</span></span>
|<span data-ttu-id="b76ef-144">Relação</span><span class="sxs-lookup"><span data-stu-id="b76ef-144">Relationship</span></span>|<span data-ttu-id="b76ef-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="b76ef-145">Type</span></span>|<span data-ttu-id="b76ef-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="b76ef-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b76ef-147">device</span><span class="sxs-lookup"><span data-stu-id="b76ef-147">device</span></span>|[<span data-ttu-id="b76ef-148">device</span><span class="sxs-lookup"><span data-stu-id="b76ef-148">device</span></span>](../resources/device.md)|<span data-ttu-id="b76ef-149">O dispositivo registrado no qual o Microsoft Authenticator reside.</span><span class="sxs-lookup"><span data-stu-id="b76ef-149">The registered device on which Microsoft Authenticator resides.</span></span> <span data-ttu-id="b76ef-150">Essa propriedade será nula se o dispositivo não estiver registrado para entrada por telefone sem senha.</span><span class="sxs-lookup"><span data-stu-id="b76ef-150">This property is null if the device is not registered for passwordless Phone Sign-In.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b76ef-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b76ef-151">JSON representation</span></span>
<span data-ttu-id="b76ef-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b76ef-152">The following is a JSON representation of the resource.</span></span>
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
