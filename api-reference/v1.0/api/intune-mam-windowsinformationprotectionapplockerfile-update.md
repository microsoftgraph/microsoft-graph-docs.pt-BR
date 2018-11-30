---
title: Atualizar windowsInformationProtectionAppLockerFile
description: Atualizar as propriedades de um objeto windowsInformationProtectionAppLockerFile.
ms.openlocfilehash: c54a29650dc47c5cc6e5e9535ee55846a8e3439b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006382"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="42bd0-103">Atualizar windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="42bd0-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="42bd0-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="42bd0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42bd0-105">Atualizar as propriedades de um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="42bd0-105">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="42bd0-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42bd0-106">Prerequisites</span></span>
<span data-ttu-id="42bd0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42bd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42bd0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42bd0-109">Permission type</span></span>|<span data-ttu-id="42bd0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="42bd0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42bd0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42bd0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="42bd0-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42bd0-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="42bd0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42bd0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42bd0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42bd0-114">Not supported.</span></span>|
|<span data-ttu-id="42bd0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42bd0-115">Application</span></span>|<span data-ttu-id="42bd0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42bd0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42bd0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42bd0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="request-headers"></a><span data-ttu-id="42bd0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42bd0-118">Request headers</span></span>
|<span data-ttu-id="42bd0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42bd0-119">Header</span></span>|<span data-ttu-id="42bd0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="42bd0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42bd0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="42bd0-121">Authorization</span></span>|<span data-ttu-id="42bd0-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42bd0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42bd0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="42bd0-123">Accept</span></span>|<span data-ttu-id="42bd0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="42bd0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42bd0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42bd0-125">Request body</span></span>
<span data-ttu-id="42bd0-126">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="42bd0-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="42bd0-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="42bd0-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="42bd0-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42bd0-128">Property</span></span>|<span data-ttu-id="42bd0-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="42bd0-129">Type</span></span>|<span data-ttu-id="42bd0-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="42bd0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42bd0-131">displayName</span><span class="sxs-lookup"><span data-stu-id="42bd0-131">displayName</span></span>|<span data-ttu-id="42bd0-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42bd0-132">String</span></span>|<span data-ttu-id="42bd0-133">O nome amigável</span><span class="sxs-lookup"><span data-stu-id="42bd0-133">The friendly name</span></span>|
|<span data-ttu-id="42bd0-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="42bd0-134">fileHash</span></span>|<span data-ttu-id="42bd0-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42bd0-135">String</span></span>|<span data-ttu-id="42bd0-136">Hash SHA256 do arquivo</span><span class="sxs-lookup"><span data-stu-id="42bd0-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="42bd0-137">file</span><span class="sxs-lookup"><span data-stu-id="42bd0-137">file</span></span>|<span data-ttu-id="42bd0-138">Binário</span><span class="sxs-lookup"><span data-stu-id="42bd0-138">Binary</span></span>|<span data-ttu-id="42bd0-139">Arquivo como uma matriz de bytes</span><span class="sxs-lookup"><span data-stu-id="42bd0-139">File as a byte array</span></span>|
|<span data-ttu-id="42bd0-140">id</span><span class="sxs-lookup"><span data-stu-id="42bd0-140">id</span></span>|<span data-ttu-id="42bd0-141">String</span><span class="sxs-lookup"><span data-stu-id="42bd0-141">String</span></span>|<span data-ttu-id="42bd0-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="42bd0-142">Key of the entity.</span></span>|
|<span data-ttu-id="42bd0-143">version</span><span class="sxs-lookup"><span data-stu-id="42bd0-143">version</span></span>|<span data-ttu-id="42bd0-144">String</span><span class="sxs-lookup"><span data-stu-id="42bd0-144">String</span></span>|<span data-ttu-id="42bd0-145">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="42bd0-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="42bd0-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="42bd0-146">Response</span></span>
<span data-ttu-id="42bd0-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42bd0-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42bd0-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42bd0-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="42bd0-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42bd0-149">Request</span></span>
<span data-ttu-id="42bd0-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42bd0-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
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

### <a name="response"></a><span data-ttu-id="42bd0-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="42bd0-151">Response</span></span>
<span data-ttu-id="42bd0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42bd0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



