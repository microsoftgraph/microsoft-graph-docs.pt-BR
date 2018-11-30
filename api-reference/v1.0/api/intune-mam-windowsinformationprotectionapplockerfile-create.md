---
title: Criar windowsInformationProtectionAppLockerFile
description: Criar um novo objeto windowsInformationProtectionAppLockerFile.
ms.openlocfilehash: a5496b599506e81e10e8a1f7d502796bdcb8d0f8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006987"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="b141a-103">Criar windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="b141a-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="b141a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b141a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b141a-105">Criar um novo objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="b141a-105">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b141a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b141a-106">Prerequisites</span></span>
<span data-ttu-id="b141a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b141a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b141a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b141a-109">Permission type</span></span>|<span data-ttu-id="b141a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b141a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b141a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b141a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b141a-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b141a-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b141a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b141a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b141a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b141a-114">Not supported.</span></span>|
|<span data-ttu-id="b141a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b141a-115">Application</span></span>|<span data-ttu-id="b141a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b141a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b141a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b141a-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b141a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b141a-118">Request headers</span></span>
|<span data-ttu-id="b141a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b141a-119">Header</span></span>|<span data-ttu-id="b141a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b141a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b141a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b141a-121">Authorization</span></span>|<span data-ttu-id="b141a-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b141a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b141a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b141a-123">Accept</span></span>|<span data-ttu-id="b141a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b141a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b141a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b141a-125">Request body</span></span>
<span data-ttu-id="b141a-126">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="b141a-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="b141a-127">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="b141a-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="b141a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b141a-128">Property</span></span>|<span data-ttu-id="b141a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b141a-129">Type</span></span>|<span data-ttu-id="b141a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b141a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b141a-131">displayName</span><span class="sxs-lookup"><span data-stu-id="b141a-131">displayName</span></span>|<span data-ttu-id="b141a-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b141a-132">String</span></span>|<span data-ttu-id="b141a-133">O nome amigável</span><span class="sxs-lookup"><span data-stu-id="b141a-133">The friendly name</span></span>|
|<span data-ttu-id="b141a-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="b141a-134">fileHash</span></span>|<span data-ttu-id="b141a-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b141a-135">String</span></span>|<span data-ttu-id="b141a-136">Hash SHA256 do arquivo</span><span class="sxs-lookup"><span data-stu-id="b141a-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="b141a-137">file</span><span class="sxs-lookup"><span data-stu-id="b141a-137">file</span></span>|<span data-ttu-id="b141a-138">Binário</span><span class="sxs-lookup"><span data-stu-id="b141a-138">Binary</span></span>|<span data-ttu-id="b141a-139">Arquivo como uma matriz de bytes</span><span class="sxs-lookup"><span data-stu-id="b141a-139">File as a byte array</span></span>|
|<span data-ttu-id="b141a-140">id</span><span class="sxs-lookup"><span data-stu-id="b141a-140">id</span></span>|<span data-ttu-id="b141a-141">String</span><span class="sxs-lookup"><span data-stu-id="b141a-141">String</span></span>|<span data-ttu-id="b141a-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b141a-142">Key of the entity.</span></span>|
|<span data-ttu-id="b141a-143">version</span><span class="sxs-lookup"><span data-stu-id="b141a-143">version</span></span>|<span data-ttu-id="b141a-144">String</span><span class="sxs-lookup"><span data-stu-id="b141a-144">String</span></span>|<span data-ttu-id="b141a-145">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="b141a-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b141a-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b141a-146">Response</span></span>
<span data-ttu-id="b141a-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b141a-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b141a-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b141a-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="b141a-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b141a-149">Request</span></span>
<span data-ttu-id="b141a-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b141a-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b141a-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="b141a-151">Response</span></span>
<span data-ttu-id="b141a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b141a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



