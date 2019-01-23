---
title: Atualizar windowsInformationProtectionAppLockerFile
description: Atualizar as propriedades de um objeto windowsInformationProtectionAppLockerFile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eee21cf2a7f2ece277ab3435b566d486120a8fc1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399826"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="5292e-103">Atualizar windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="5292e-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="5292e-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="5292e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5292e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5292e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5292e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="5292e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5292e-107">Atualizar as propriedades de um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="5292e-107">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5292e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5292e-108">Prerequisites</span></span>
<span data-ttu-id="5292e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5292e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5292e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5292e-111">Permission type</span></span>|<span data-ttu-id="5292e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5292e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5292e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5292e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5292e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5292e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5292e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5292e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5292e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5292e-116">Not supported.</span></span>|
|<span data-ttu-id="5292e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5292e-117">Application</span></span>|<span data-ttu-id="5292e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5292e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5292e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5292e-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5292e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5292e-120">Request headers</span></span>
|<span data-ttu-id="5292e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5292e-121">Header</span></span>|<span data-ttu-id="5292e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5292e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5292e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5292e-123">Authorization</span></span>|<span data-ttu-id="5292e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5292e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5292e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5292e-125">Accept</span></span>|<span data-ttu-id="5292e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5292e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5292e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5292e-127">Request body</span></span>
<span data-ttu-id="5292e-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="5292e-128">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="5292e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="5292e-129">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="5292e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5292e-130">Property</span></span>|<span data-ttu-id="5292e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5292e-131">Type</span></span>|<span data-ttu-id="5292e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5292e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5292e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5292e-133">displayName</span></span>|<span data-ttu-id="5292e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5292e-134">String</span></span>|<span data-ttu-id="5292e-135">O nome amigável</span><span class="sxs-lookup"><span data-stu-id="5292e-135">The friendly name</span></span>|
|<span data-ttu-id="5292e-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="5292e-136">fileHash</span></span>|<span data-ttu-id="5292e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5292e-137">String</span></span>|<span data-ttu-id="5292e-138">Hash SHA256 do arquivo</span><span class="sxs-lookup"><span data-stu-id="5292e-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="5292e-139">file</span><span class="sxs-lookup"><span data-stu-id="5292e-139">file</span></span>|<span data-ttu-id="5292e-140">Binária</span><span class="sxs-lookup"><span data-stu-id="5292e-140">Binary</span></span>|<span data-ttu-id="5292e-141">Arquivo como uma matriz de bytes</span><span class="sxs-lookup"><span data-stu-id="5292e-141">File as a byte array</span></span>|
|<span data-ttu-id="5292e-142">id</span><span class="sxs-lookup"><span data-stu-id="5292e-142">id</span></span>|<span data-ttu-id="5292e-143">String</span><span class="sxs-lookup"><span data-stu-id="5292e-143">String</span></span>|<span data-ttu-id="5292e-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5292e-144">Key of the entity.</span></span>|
|<span data-ttu-id="5292e-145">version</span><span class="sxs-lookup"><span data-stu-id="5292e-145">version</span></span>|<span data-ttu-id="5292e-146">String</span><span class="sxs-lookup"><span data-stu-id="5292e-146">String</span></span>|<span data-ttu-id="5292e-147">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="5292e-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="5292e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="5292e-148">Response</span></span>
<span data-ttu-id="5292e-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5292e-149">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5292e-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5292e-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="5292e-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5292e-151">Request</span></span>
<span data-ttu-id="5292e-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5292e-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5292e-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="5292e-153">Response</span></span>
<span data-ttu-id="5292e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5292e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




