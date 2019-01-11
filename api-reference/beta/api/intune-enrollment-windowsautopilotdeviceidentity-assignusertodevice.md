---
title: ação de assignUserToDevice
description: Atribui o usuário a dispositivos de piloto automático.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 33145d5852d80eef529cc58e34524c170bba62cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859455"
---
# <a name="assignusertodevice-action"></a><span data-ttu-id="19122-103">ação de assignUserToDevice</span><span class="sxs-lookup"><span data-stu-id="19122-103">assignUserToDevice action</span></span>

> <span data-ttu-id="19122-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="19122-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19122-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="19122-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19122-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="19122-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19122-107">Atribui o usuário a dispositivos de piloto automático.</span><span class="sxs-lookup"><span data-stu-id="19122-107">Assigns user to Autopilot devices.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="19122-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="19122-108">Prerequisites</span></span>
<span data-ttu-id="19122-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19122-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19122-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19122-111">Permission type</span></span>|<span data-ttu-id="19122-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="19122-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19122-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19122-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19122-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19122-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="19122-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19122-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19122-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19122-116">Not supported.</span></span>|
|<span data-ttu-id="19122-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19122-117">Application</span></span>|<span data-ttu-id="19122-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19122-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19122-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19122-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
```

## <a name="request-headers"></a><span data-ttu-id="19122-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19122-120">Request headers</span></span>
|<span data-ttu-id="19122-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="19122-121">Header</span></span>|<span data-ttu-id="19122-122">Valor</span><span class="sxs-lookup"><span data-stu-id="19122-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19122-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="19122-123">Authorization</span></span>|<span data-ttu-id="19122-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19122-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19122-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="19122-125">Accept</span></span>|<span data-ttu-id="19122-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19122-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19122-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19122-127">Request body</span></span>
<span data-ttu-id="19122-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="19122-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="19122-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="19122-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="19122-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19122-130">Property</span></span>|<span data-ttu-id="19122-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="19122-131">Type</span></span>|<span data-ttu-id="19122-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="19122-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19122-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="19122-133">userPrincipalName</span></span>|<span data-ttu-id="19122-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19122-134">String</span></span>|<span data-ttu-id="19122-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="19122-135">Not yet documented</span></span>|
|<span data-ttu-id="19122-136">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="19122-136">addressableUserName</span></span>|<span data-ttu-id="19122-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19122-137">String</span></span>|<span data-ttu-id="19122-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="19122-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="19122-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="19122-139">Response</span></span>
<span data-ttu-id="19122-140">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="19122-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="19122-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19122-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="19122-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19122-142">Request</span></span>
<span data-ttu-id="19122-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19122-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice

Content-type: application/json
Content-length: 113

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value"
}
```

### <a name="response"></a><span data-ttu-id="19122-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="19122-144">Response</span></span>
<span data-ttu-id="19122-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19122-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





