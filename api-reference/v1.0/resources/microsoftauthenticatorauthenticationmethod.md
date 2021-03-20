---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethod
description: Uma representação do aplicativo Microsoft Authenticator registrado para um usuário. O Microsoft Authenticator é um método de autenticação.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aeb2d1d7b111c9424da2f927dbaf3030a356c6b6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964573"
---
# <a name="microsoftauthenticatorauthenticationmethod-resource-type"></a><span data-ttu-id="142a9-104">Tipo de recurso microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="142a9-104">microsoftAuthenticatorAuthenticationMethod resource type</span></span>

<span data-ttu-id="142a9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="142a9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="142a9-106">Uma representação do aplicativo Microsoft Authenticator registrado para um usuário.</span><span class="sxs-lookup"><span data-stu-id="142a9-106">A representation of the Microsoft Authenticator app registered to a user.</span></span> <span data-ttu-id="142a9-107">O Microsoft Authenticator é um método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="142a9-107">Microsoft Authenticator is an authentication method.</span></span>

<span data-ttu-id="142a9-108">Herda de [authenticationMethod](../resources/authenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="142a9-108">Inherits from [authenticationMethod](../resources/authenticationmethod.md).</span></span>

## <a name="methods"></a><span data-ttu-id="142a9-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="142a9-109">Methods</span></span>
|<span data-ttu-id="142a9-110">Método</span><span class="sxs-lookup"><span data-stu-id="142a9-110">Method</span></span>|<span data-ttu-id="142a9-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="142a9-111">Return type</span></span>|<span data-ttu-id="142a9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="142a9-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="142a9-113">Listar microsoftAuthenticatorAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="142a9-113">List microsoftAuthenticatorAuthenticationMethods</span></span>](../api/microsoftauthenticatorauthenticationmethod-list.md)|<span data-ttu-id="142a9-114">[coleção microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="142a9-114">[microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) collection</span></span>|<span data-ttu-id="142a9-115">Obter uma lista dos [objetos microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="142a9-115">Get a list of the [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>|
|[<span data-ttu-id="142a9-116">Obter microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="142a9-116">Get microsoftAuthenticatorAuthenticationMethod</span></span>](../api/microsoftauthenticatorauthenticationmethod-get.md)|[<span data-ttu-id="142a9-117">microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="142a9-117">microsoftAuthenticatorAuthenticationMethod</span></span>](../resources/microsoftauthenticatorauthenticationmethod.md)|<span data-ttu-id="142a9-118">Leia as propriedades e as relações de um [objeto microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="142a9-118">Read the properties and relationships of a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>|
|[<span data-ttu-id="142a9-119">Excluir microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="142a9-119">Delete microsoftAuthenticatorAuthenticationMethod</span></span>](../api/microsoftauthenticatorauthenticationmethod-delete.md)|<span data-ttu-id="142a9-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="142a9-120">None</span></span>|<span data-ttu-id="142a9-121">Exclui um [objeto microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="142a9-121">Deletes a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="142a9-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="142a9-122">Properties</span></span>
|<span data-ttu-id="142a9-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="142a9-123">Property</span></span>|<span data-ttu-id="142a9-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="142a9-124">Type</span></span>|<span data-ttu-id="142a9-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="142a9-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="142a9-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="142a9-126">createdDateTime</span></span>|<span data-ttu-id="142a9-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="142a9-127">DateTimeOffset</span></span>|<span data-ttu-id="142a9-128">A data e a hora em que esse aplicativo foi registrado.</span><span class="sxs-lookup"><span data-stu-id="142a9-128">The date and time that this app was registered.</span></span> <span data-ttu-id="142a9-129">Essa propriedade será nula se o dispositivo não estiver registrado para Entrada de Telefone sem senha.</span><span class="sxs-lookup"><span data-stu-id="142a9-129">This property is null if the device is not registered for passwordless Phone Sign-In.</span></span>|
|<span data-ttu-id="142a9-130">displayName</span><span class="sxs-lookup"><span data-stu-id="142a9-130">displayName</span></span>|<span data-ttu-id="142a9-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="142a9-131">String</span></span>|<span data-ttu-id="142a9-132">O nome do dispositivo no qual esse aplicativo está registrado.</span><span class="sxs-lookup"><span data-stu-id="142a9-132">The name of the device on which this app is registered.</span></span>|
|<span data-ttu-id="142a9-133">id</span><span class="sxs-lookup"><span data-stu-id="142a9-133">id</span></span>|<span data-ttu-id="142a9-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="142a9-134">String</span></span>|<span data-ttu-id="142a9-135">Um identificador exclusivo para esse método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="142a9-135">A unique identifier for this authentication method.</span></span> <span data-ttu-id="142a9-136">Herdado da [autenticaçãoMethod](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="142a9-136">Inherited from [authenticationMethod](../resources/authenticationmethod.md)</span></span>|
|<span data-ttu-id="142a9-137">deviceTag</span><span class="sxs-lookup"><span data-stu-id="142a9-137">deviceTag</span></span>|<span data-ttu-id="142a9-138">String</span><span class="sxs-lookup"><span data-stu-id="142a9-138">String</span></span>|<span data-ttu-id="142a9-139">Marcas que contêm metadados de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="142a9-139">Tags containing app metadata.</span></span>|
|<span data-ttu-id="142a9-140">phoneAppVersion</span><span class="sxs-lookup"><span data-stu-id="142a9-140">phoneAppVersion</span></span>|<span data-ttu-id="142a9-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="142a9-141">String</span></span>|<span data-ttu-id="142a9-142">Versão numérica dessa instância do aplicativo Authenticator.</span><span class="sxs-lookup"><span data-stu-id="142a9-142">Numerical version of this instance of the Authenticator app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="142a9-143">Relações</span><span class="sxs-lookup"><span data-stu-id="142a9-143">Relationships</span></span>
|<span data-ttu-id="142a9-144">Relação</span><span class="sxs-lookup"><span data-stu-id="142a9-144">Relationship</span></span>|<span data-ttu-id="142a9-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="142a9-145">Type</span></span>|<span data-ttu-id="142a9-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="142a9-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="142a9-147">device</span><span class="sxs-lookup"><span data-stu-id="142a9-147">device</span></span>|[<span data-ttu-id="142a9-148">device</span><span class="sxs-lookup"><span data-stu-id="142a9-148">device</span></span>](../resources/device.md)|<span data-ttu-id="142a9-149">O dispositivo registrado no qual o Microsoft Authenticator reside.</span><span class="sxs-lookup"><span data-stu-id="142a9-149">The registered device on which Microsoft Authenticator resides.</span></span> <span data-ttu-id="142a9-150">Essa propriedade será nula se o dispositivo não estiver registrado para Entrada de Telefone sem senha.</span><span class="sxs-lookup"><span data-stu-id="142a9-150">This property is null if the device is not registered for passwordless Phone Sign-In.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="142a9-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="142a9-151">JSON representation</span></span>
<span data-ttu-id="142a9-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="142a9-152">The following is a JSON representation of the resource.</span></span>
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
