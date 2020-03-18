---
title: Criar windowsDefenderApplicationControlSupplementalPolicy
description: Criar um novo objeto windowsDefenderApplicationControlSupplementalPolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d207aaced3212111cc40c78576fffe3ceb9d21ad
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800071"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicy"></a><span data-ttu-id="3797d-103">Criar windowsDefenderApplicationControlSupplementalPolicy</span><span class="sxs-lookup"><span data-stu-id="3797d-103">Create windowsDefenderApplicationControlSupplementalPolicy</span></span>

> <span data-ttu-id="3797d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3797d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3797d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3797d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3797d-106">Criar um novo objeto [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="3797d-106">Create a new [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3797d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3797d-107">Prerequisites</span></span>
<span data-ttu-id="3797d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3797d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3797d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3797d-110">Permission type</span></span>|<span data-ttu-id="3797d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3797d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3797d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3797d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3797d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3797d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3797d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3797d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3797d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3797d-115">Not supported.</span></span>|
|<span data-ttu-id="3797d-116">Application</span><span class="sxs-lookup"><span data-stu-id="3797d-116">Application</span></span>|<span data-ttu-id="3797d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3797d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3797d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3797d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies
```

## <a name="request-headers"></a><span data-ttu-id="3797d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3797d-119">Request headers</span></span>
|<span data-ttu-id="3797d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3797d-120">Header</span></span>|<span data-ttu-id="3797d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3797d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3797d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3797d-122">Authorization</span></span>|<span data-ttu-id="3797d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3797d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3797d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3797d-124">Accept</span></span>|<span data-ttu-id="3797d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3797d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3797d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3797d-126">Request body</span></span>
<span data-ttu-id="3797d-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsDefenderApplicationControlSupplementalPolicy.</span><span class="sxs-lookup"><span data-stu-id="3797d-127">In the request body, supply a JSON representation for the windowsDefenderApplicationControlSupplementalPolicy object.</span></span>

<span data-ttu-id="3797d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDefenderApplicationControlSupplementalPolicy.</span><span class="sxs-lookup"><span data-stu-id="3797d-128">The following table shows the properties that are required when you create the windowsDefenderApplicationControlSupplementalPolicy.</span></span>

|<span data-ttu-id="3797d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3797d-129">Property</span></span>|<span data-ttu-id="3797d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3797d-130">Type</span></span>|<span data-ttu-id="3797d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3797d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3797d-132">id</span><span class="sxs-lookup"><span data-stu-id="3797d-132">id</span></span>|<span data-ttu-id="3797d-133">String</span><span class="sxs-lookup"><span data-stu-id="3797d-133">String</span></span>|<span data-ttu-id="3797d-134">A chave da política complementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="3797d-134">The key for the WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="3797d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3797d-135">displayName</span></span>|<span data-ttu-id="3797d-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3797d-136">String</span></span>|<span data-ttu-id="3797d-137">O nome de exibição da política complementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="3797d-137">The display name of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="3797d-138">description</span><span class="sxs-lookup"><span data-stu-id="3797d-138">description</span></span>|<span data-ttu-id="3797d-139">String</span><span class="sxs-lookup"><span data-stu-id="3797d-139">String</span></span>|<span data-ttu-id="3797d-140">A descrição da política suplementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="3797d-140">The description of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="3797d-141">conteúdo</span><span class="sxs-lookup"><span data-stu-id="3797d-141">content</span></span>|<span data-ttu-id="3797d-142">Binária</span><span class="sxs-lookup"><span data-stu-id="3797d-142">Binary</span></span>|<span data-ttu-id="3797d-143">O conteúdo de política suplementar WindowsDefenderApplicationControl no formato de matriz de bytes.</span><span class="sxs-lookup"><span data-stu-id="3797d-143">The WindowsDefenderApplicationControl supplemental policy content in byte array format.</span></span>|
|<span data-ttu-id="3797d-144">contentFileName</span><span class="sxs-lookup"><span data-stu-id="3797d-144">contentFileName</span></span>|<span data-ttu-id="3797d-145">String</span><span class="sxs-lookup"><span data-stu-id="3797d-145">String</span></span>|<span data-ttu-id="3797d-146">O nome de arquivo do conteúdo da política suplementar da WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="3797d-146">The WindowsDefenderApplicationControl supplemental policy content's file name.</span></span>|
|<span data-ttu-id="3797d-147">versão</span><span class="sxs-lookup"><span data-stu-id="3797d-147">version</span></span>|<span data-ttu-id="3797d-148">String</span><span class="sxs-lookup"><span data-stu-id="3797d-148">String</span></span>|<span data-ttu-id="3797d-149">A versão da política suplementar da WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="3797d-149">The WindowsDefenderApplicationControl supplemental policy's version.</span></span>|
|<span data-ttu-id="3797d-150">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="3797d-150">creationDateTime</span></span>|<span data-ttu-id="3797d-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3797d-151">DateTimeOffset</span></span>|<span data-ttu-id="3797d-152">A data e a hora em que a política suplementar WindowsDefenderApplicationControl foi carregada.</span><span class="sxs-lookup"><span data-stu-id="3797d-152">The date and time when the WindowsDefenderApplicationControl supplemental policy was uploaded.</span></span>|
|<span data-ttu-id="3797d-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3797d-153">lastModifiedDateTime</span></span>|<span data-ttu-id="3797d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3797d-154">DateTimeOffset</span></span>|<span data-ttu-id="3797d-155">A data e a hora da última modificação da política suplementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="3797d-155">The date and time when the WindowsDefenderApplicationControl supplemental policy was last modified.</span></span>|
|<span data-ttu-id="3797d-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3797d-156">roleScopeTagIds</span></span>|<span data-ttu-id="3797d-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3797d-157">String collection</span></span>|<span data-ttu-id="3797d-158">Lista de marcas de escopo para esta entidade de política suplementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="3797d-158">List of Scope Tags for this WindowsDefenderApplicationControl supplemental policy entity.</span></span>|



## <a name="response"></a><span data-ttu-id="3797d-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="3797d-159">Response</span></span>
<span data-ttu-id="3797d-160">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3797d-160">If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3797d-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3797d-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="3797d-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3797d-162">Request</span></span>
<span data-ttu-id="3797d-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3797d-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "content": "Y29udGVudA==",
  "contentFileName": "Content File Name value",
  "version": "Version value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="3797d-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="3797d-164">Response</span></span>
<span data-ttu-id="3797d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3797d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 517

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "id": "83d0c39e-c39e-83d0-9ec3-d0839ec3d083",
  "displayName": "Display Name value",
  "description": "Description value",
  "content": "Y29udGVudA==",
  "contentFileName": "Content File Name value",
  "version": "Version value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




