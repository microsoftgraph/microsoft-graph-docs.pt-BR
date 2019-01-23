---
title: Ação wipe
description: Apagar um dispositivo
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 56ee058ee4ea6c5760707f895d626b35163c68ba
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398706"
---
# <a name="wipe-action"></a><span data-ttu-id="76f21-103">Ação wipe</span><span class="sxs-lookup"><span data-stu-id="76f21-103">wipe action</span></span>

> <span data-ttu-id="76f21-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="76f21-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="76f21-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="76f21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="76f21-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="76f21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76f21-107">Apagar um dispositivo</span><span class="sxs-lookup"><span data-stu-id="76f21-107">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76f21-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="76f21-108">Prerequisites</span></span>
<span data-ttu-id="76f21-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="76f21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="76f21-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76f21-111">Permission type</span></span>|<span data-ttu-id="76f21-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="76f21-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76f21-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76f21-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76f21-114">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76f21-114">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="76f21-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76f21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76f21-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76f21-116">Not supported.</span></span>|
|<span data-ttu-id="76f21-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76f21-117">Application</span></span>|<span data-ttu-id="76f21-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76f21-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76f21-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76f21-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="76f21-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76f21-120">Request headers</span></span>
|<span data-ttu-id="76f21-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76f21-121">Header</span></span>|<span data-ttu-id="76f21-122">Valor</span><span class="sxs-lookup"><span data-stu-id="76f21-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76f21-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="76f21-123">Authorization</span></span>|<span data-ttu-id="76f21-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76f21-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76f21-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="76f21-125">Accept</span></span>|<span data-ttu-id="76f21-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76f21-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76f21-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76f21-127">Request body</span></span>
<span data-ttu-id="76f21-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="76f21-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="76f21-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="76f21-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="76f21-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76f21-130">Property</span></span>|<span data-ttu-id="76f21-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="76f21-131">Type</span></span>|<span data-ttu-id="76f21-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="76f21-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76f21-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="76f21-133">keepEnrollmentData</span></span>|<span data-ttu-id="76f21-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="76f21-134">Boolean</span></span>|<span data-ttu-id="76f21-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="76f21-135">Not yet documented</span></span>|
|<span data-ttu-id="76f21-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="76f21-136">keepUserData</span></span>|<span data-ttu-id="76f21-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="76f21-137">Boolean</span></span>|<span data-ttu-id="76f21-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="76f21-138">Not yet documented</span></span>|
|<span data-ttu-id="76f21-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="76f21-139">macOsUnlockCode</span></span>|<span data-ttu-id="76f21-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76f21-140">String</span></span>|<span data-ttu-id="76f21-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="76f21-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="76f21-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="76f21-142">Response</span></span>
<span data-ttu-id="76f21-143">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="76f21-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="76f21-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76f21-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="76f21-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76f21-145">Request</span></span>
<span data-ttu-id="76f21-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76f21-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="76f21-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="76f21-147">Response</span></span>
<span data-ttu-id="76f21-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76f21-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




