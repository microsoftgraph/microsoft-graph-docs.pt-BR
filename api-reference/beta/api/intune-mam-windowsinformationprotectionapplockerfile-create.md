---
title: Criar windowsInformationProtectionAppLockerFile
description: Criar um novo objeto windowsInformationProtectionAppLockerFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d396416da77cc0469fb2e295f3527f39b950d5d9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49277250"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="c6481-103">Criar windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="c6481-103">Create windowsInformationProtectionAppLockerFile</span></span>

<span data-ttu-id="c6481-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6481-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6481-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c6481-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6481-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c6481-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6481-107">Criar um novo objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="c6481-107">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6481-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c6481-108">Prerequisites</span></span>
<span data-ttu-id="c6481-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6481-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6481-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6481-111">Permission type</span></span>|<span data-ttu-id="c6481-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c6481-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6481-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6481-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c6481-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6481-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c6481-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6481-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6481-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6481-116">Not supported.</span></span>|
|<span data-ttu-id="c6481-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6481-117">Application</span></span>|<span data-ttu-id="c6481-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6481-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6481-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6481-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c6481-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6481-120">Request headers</span></span>
|<span data-ttu-id="c6481-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6481-121">Header</span></span>|<span data-ttu-id="c6481-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c6481-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6481-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6481-123">Authorization</span></span>|<span data-ttu-id="c6481-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6481-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6481-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c6481-125">Accept</span></span>|<span data-ttu-id="c6481-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6481-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6481-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6481-127">Request body</span></span>
<span data-ttu-id="c6481-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="c6481-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="c6481-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="c6481-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="c6481-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6481-130">Property</span></span>|<span data-ttu-id="c6481-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6481-131">Type</span></span>|<span data-ttu-id="c6481-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6481-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6481-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c6481-133">displayName</span></span>|<span data-ttu-id="c6481-134">String</span><span class="sxs-lookup"><span data-stu-id="c6481-134">String</span></span>|<span data-ttu-id="c6481-135">O nome amigável</span><span class="sxs-lookup"><span data-stu-id="c6481-135">The friendly name</span></span>|
|<span data-ttu-id="c6481-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="c6481-136">fileHash</span></span>|<span data-ttu-id="c6481-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6481-137">String</span></span>|<span data-ttu-id="c6481-138">Hash SHA256 do arquivo</span><span class="sxs-lookup"><span data-stu-id="c6481-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="c6481-139">file</span><span class="sxs-lookup"><span data-stu-id="c6481-139">file</span></span>|<span data-ttu-id="c6481-140">Binária</span><span class="sxs-lookup"><span data-stu-id="c6481-140">Binary</span></span>|<span data-ttu-id="c6481-141">Arquivo como uma matriz de bytes</span><span class="sxs-lookup"><span data-stu-id="c6481-141">File as a byte array</span></span>|
|<span data-ttu-id="c6481-142">id</span><span class="sxs-lookup"><span data-stu-id="c6481-142">id</span></span>|<span data-ttu-id="c6481-143">String</span><span class="sxs-lookup"><span data-stu-id="c6481-143">String</span></span>|<span data-ttu-id="c6481-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c6481-144">Key of the entity.</span></span>|
|<span data-ttu-id="c6481-145">versão</span><span class="sxs-lookup"><span data-stu-id="c6481-145">version</span></span>|<span data-ttu-id="c6481-146">String</span><span class="sxs-lookup"><span data-stu-id="c6481-146">String</span></span>|<span data-ttu-id="c6481-147">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="c6481-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="c6481-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6481-148">Response</span></span>
<span data-ttu-id="c6481-149">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6481-149">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6481-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6481-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6481-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6481-151">Request</span></span>
<span data-ttu-id="c6481-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6481-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c6481-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6481-153">Response</span></span>
<span data-ttu-id="c6481-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6481-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




