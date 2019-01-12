---
title: Criar windowsInformationProtectionAppLockerFile
description: Criar um novo objeto windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a7b6bfb8271e6b462be1d18fd509da33aea836b3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967592"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="41977-103">Criar windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="41977-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="41977-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="41977-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41977-105">Criar um novo objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="41977-105">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41977-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41977-106">Prerequisites</span></span>
<span data-ttu-id="41977-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41977-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41977-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41977-109">Permission type</span></span>|<span data-ttu-id="41977-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="41977-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41977-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41977-111">Delegated (work or school account)</span></span>|<span data-ttu-id="41977-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41977-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="41977-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41977-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41977-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41977-114">Not supported.</span></span>|
|<span data-ttu-id="41977-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41977-115">Application</span></span>|<span data-ttu-id="41977-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41977-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41977-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41977-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a><span data-ttu-id="41977-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41977-118">Request headers</span></span>
|<span data-ttu-id="41977-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41977-119">Header</span></span>|<span data-ttu-id="41977-120">Valor</span><span class="sxs-lookup"><span data-stu-id="41977-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41977-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="41977-121">Authorization</span></span>|<span data-ttu-id="41977-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41977-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41977-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="41977-123">Accept</span></span>|<span data-ttu-id="41977-124">application/json</span><span class="sxs-lookup"><span data-stu-id="41977-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41977-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41977-125">Request body</span></span>
<span data-ttu-id="41977-126">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="41977-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="41977-127">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="41977-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="41977-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41977-128">Property</span></span>|<span data-ttu-id="41977-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="41977-129">Type</span></span>|<span data-ttu-id="41977-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="41977-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41977-131">displayName</span><span class="sxs-lookup"><span data-stu-id="41977-131">displayName</span></span>|<span data-ttu-id="41977-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41977-132">String</span></span>|<span data-ttu-id="41977-133">O nome amigável</span><span class="sxs-lookup"><span data-stu-id="41977-133">The friendly name</span></span>|
|<span data-ttu-id="41977-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="41977-134">fileHash</span></span>|<span data-ttu-id="41977-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41977-135">String</span></span>|<span data-ttu-id="41977-136">Hash SHA256 do arquivo</span><span class="sxs-lookup"><span data-stu-id="41977-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="41977-137">file</span><span class="sxs-lookup"><span data-stu-id="41977-137">file</span></span>|<span data-ttu-id="41977-138">Binária</span><span class="sxs-lookup"><span data-stu-id="41977-138">Binary</span></span>|<span data-ttu-id="41977-139">Arquivo como uma matriz de bytes</span><span class="sxs-lookup"><span data-stu-id="41977-139">File as a byte array</span></span>|
|<span data-ttu-id="41977-140">id</span><span class="sxs-lookup"><span data-stu-id="41977-140">id</span></span>|<span data-ttu-id="41977-141">String</span><span class="sxs-lookup"><span data-stu-id="41977-141">String</span></span>|<span data-ttu-id="41977-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="41977-142">Key of the entity.</span></span>|
|<span data-ttu-id="41977-143">version</span><span class="sxs-lookup"><span data-stu-id="41977-143">version</span></span>|<span data-ttu-id="41977-144">String</span><span class="sxs-lookup"><span data-stu-id="41977-144">String</span></span>|<span data-ttu-id="41977-145">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="41977-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="41977-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="41977-146">Response</span></span>
<span data-ttu-id="41977-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41977-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41977-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41977-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="41977-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41977-149">Request</span></span>
<span data-ttu-id="41977-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41977-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="41977-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="41977-151">Response</span></span>
<span data-ttu-id="41977-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41977-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
  "version": "Version value"
}
```



