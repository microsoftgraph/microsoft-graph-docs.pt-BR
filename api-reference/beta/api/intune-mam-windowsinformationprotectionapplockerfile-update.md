---
title: Atualizar windowsInformationProtectionAppLockerFile
description: Atualizar as propriedades de um objeto windowsInformationProtectionAppLockerFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3754ca665f755f0adc83b59001176ccb84b4f779
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078686"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="d84ac-103">Atualizar windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="d84ac-103">Update windowsInformationProtectionAppLockerFile</span></span>

<span data-ttu-id="d84ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d84ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d84ac-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d84ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d84ac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d84ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d84ac-107">Atualizar as propriedades de um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="d84ac-107">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d84ac-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d84ac-108">Prerequisites</span></span>
<span data-ttu-id="d84ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d84ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d84ac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d84ac-111">Permission type</span></span>|<span data-ttu-id="d84ac-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d84ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d84ac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d84ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d84ac-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d84ac-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d84ac-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d84ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d84ac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d84ac-116">Not supported.</span></span>|
|<span data-ttu-id="d84ac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d84ac-117">Application</span></span>|<span data-ttu-id="d84ac-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d84ac-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d84ac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d84ac-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d84ac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d84ac-120">Request headers</span></span>
|<span data-ttu-id="d84ac-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d84ac-121">Header</span></span>|<span data-ttu-id="d84ac-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d84ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d84ac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d84ac-123">Authorization</span></span>|<span data-ttu-id="d84ac-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d84ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d84ac-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d84ac-125">Accept</span></span>|<span data-ttu-id="d84ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d84ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d84ac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d84ac-127">Request body</span></span>
<span data-ttu-id="d84ac-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="d84ac-128">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="d84ac-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="d84ac-129">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="d84ac-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d84ac-130">Property</span></span>|<span data-ttu-id="d84ac-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d84ac-131">Type</span></span>|<span data-ttu-id="d84ac-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d84ac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d84ac-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d84ac-133">displayName</span></span>|<span data-ttu-id="d84ac-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d84ac-134">String</span></span>|<span data-ttu-id="d84ac-135">O nome amigável</span><span class="sxs-lookup"><span data-stu-id="d84ac-135">The friendly name</span></span>|
|<span data-ttu-id="d84ac-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="d84ac-136">fileHash</span></span>|<span data-ttu-id="d84ac-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d84ac-137">String</span></span>|<span data-ttu-id="d84ac-138">Hash SHA256 do arquivo</span><span class="sxs-lookup"><span data-stu-id="d84ac-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="d84ac-139">file</span><span class="sxs-lookup"><span data-stu-id="d84ac-139">file</span></span>|<span data-ttu-id="d84ac-140">Binária</span><span class="sxs-lookup"><span data-stu-id="d84ac-140">Binary</span></span>|<span data-ttu-id="d84ac-141">Arquivo como uma matriz de bytes</span><span class="sxs-lookup"><span data-stu-id="d84ac-141">File as a byte array</span></span>|
|<span data-ttu-id="d84ac-142">id</span><span class="sxs-lookup"><span data-stu-id="d84ac-142">id</span></span>|<span data-ttu-id="d84ac-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d84ac-143">String</span></span>|<span data-ttu-id="d84ac-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d84ac-144">Key of the entity.</span></span>|
|<span data-ttu-id="d84ac-145">versão</span><span class="sxs-lookup"><span data-stu-id="d84ac-145">version</span></span>|<span data-ttu-id="d84ac-146">String</span><span class="sxs-lookup"><span data-stu-id="d84ac-146">String</span></span>|<span data-ttu-id="d84ac-147">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="d84ac-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="d84ac-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="d84ac-148">Response</span></span>
<span data-ttu-id="d84ac-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d84ac-149">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d84ac-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d84ac-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="d84ac-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d84ac-151">Request</span></span>
<span data-ttu-id="d84ac-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d84ac-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
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

### <a name="response"></a><span data-ttu-id="d84ac-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d84ac-153">Response</span></span>
<span data-ttu-id="d84ac-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d84ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






