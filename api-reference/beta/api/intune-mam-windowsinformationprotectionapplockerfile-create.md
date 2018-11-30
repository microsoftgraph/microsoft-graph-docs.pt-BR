---
title: Criar windowsInformationProtectionAppLockerFile
description: Criar um novo objeto windowsInformationProtectionAppLockerFile.
ms.openlocfilehash: 380b4b9358c3bc30337272ced4b92563978d7ffe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037797"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="e44ae-103">Criar windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="e44ae-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="e44ae-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e44ae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e44ae-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e44ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e44ae-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e44ae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e44ae-107">Criar um novo objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="e44ae-107">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e44ae-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e44ae-108">Prerequisites</span></span>
<span data-ttu-id="e44ae-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e44ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e44ae-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e44ae-111">Permission type</span></span>|<span data-ttu-id="e44ae-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e44ae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e44ae-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e44ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e44ae-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e44ae-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e44ae-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e44ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e44ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e44ae-116">Not supported.</span></span>|
|<span data-ttu-id="e44ae-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e44ae-117">Application</span></span>|<span data-ttu-id="e44ae-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e44ae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e44ae-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e44ae-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e44ae-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e44ae-120">Request headers</span></span>
|<span data-ttu-id="e44ae-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e44ae-121">Header</span></span>|<span data-ttu-id="e44ae-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e44ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e44ae-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e44ae-123">Authorization</span></span>|<span data-ttu-id="e44ae-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e44ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e44ae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e44ae-125">Accept</span></span>|<span data-ttu-id="e44ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e44ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e44ae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e44ae-127">Request body</span></span>
<span data-ttu-id="e44ae-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="e44ae-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="e44ae-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="e44ae-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="e44ae-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e44ae-130">Property</span></span>|<span data-ttu-id="e44ae-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e44ae-131">Type</span></span>|<span data-ttu-id="e44ae-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e44ae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e44ae-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e44ae-133">displayName</span></span>|<span data-ttu-id="e44ae-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e44ae-134">String</span></span>|<span data-ttu-id="e44ae-135">O nome amigável</span><span class="sxs-lookup"><span data-stu-id="e44ae-135">The friendly name</span></span>|
|<span data-ttu-id="e44ae-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="e44ae-136">fileHash</span></span>|<span data-ttu-id="e44ae-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e44ae-137">String</span></span>|<span data-ttu-id="e44ae-138">Hash SHA256 do arquivo</span><span class="sxs-lookup"><span data-stu-id="e44ae-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="e44ae-139">file</span><span class="sxs-lookup"><span data-stu-id="e44ae-139">file</span></span>|<span data-ttu-id="e44ae-140">Binário</span><span class="sxs-lookup"><span data-stu-id="e44ae-140">Binary</span></span>|<span data-ttu-id="e44ae-141">Arquivo como uma matriz de bytes</span><span class="sxs-lookup"><span data-stu-id="e44ae-141">File as a byte array</span></span>|
|<span data-ttu-id="e44ae-142">id</span><span class="sxs-lookup"><span data-stu-id="e44ae-142">id</span></span>|<span data-ttu-id="e44ae-143">String</span><span class="sxs-lookup"><span data-stu-id="e44ae-143">String</span></span>|<span data-ttu-id="e44ae-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e44ae-144">Key of the entity.</span></span>|
|<span data-ttu-id="e44ae-145">version</span><span class="sxs-lookup"><span data-stu-id="e44ae-145">version</span></span>|<span data-ttu-id="e44ae-146">String</span><span class="sxs-lookup"><span data-stu-id="e44ae-146">String</span></span>|<span data-ttu-id="e44ae-147">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="e44ae-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="e44ae-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e44ae-148">Response</span></span>
<span data-ttu-id="e44ae-149">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e44ae-149">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e44ae-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e44ae-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="e44ae-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e44ae-151">Request</span></span>
<span data-ttu-id="e44ae-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e44ae-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
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

### <a name="response"></a><span data-ttu-id="e44ae-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="e44ae-153">Response</span></span>
<span data-ttu-id="e44ae-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e44ae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





