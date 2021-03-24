---
title: Atualizar windowsDefenderApplicationControlSupplementalPolicy
description: Atualize as propriedades de um objeto windowsDefenderApplicationControlSupplementalPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c6740654616d112db2d64910b5dd716111a582c0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134022"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicy"></a><span data-ttu-id="1719a-103">Atualizar windowsDefenderApplicationControlSupplementalPolicy</span><span class="sxs-lookup"><span data-stu-id="1719a-103">Update windowsDefenderApplicationControlSupplementalPolicy</span></span>

<span data-ttu-id="1719a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1719a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1719a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1719a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1719a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1719a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1719a-107">Atualize as propriedades de um [objeto windowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1719a-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1719a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1719a-108">Prerequisites</span></span>
<span data-ttu-id="1719a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1719a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1719a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1719a-111">Permission type</span></span>|<span data-ttu-id="1719a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1719a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1719a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1719a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1719a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1719a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1719a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1719a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1719a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1719a-116">Not supported.</span></span>|
|<span data-ttu-id="1719a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1719a-117">Application</span></span>|<span data-ttu-id="1719a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1719a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1719a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1719a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}/policy
```

## <a name="request-headers"></a><span data-ttu-id="1719a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1719a-120">Request headers</span></span>
|<span data-ttu-id="1719a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1719a-121">Header</span></span>|<span data-ttu-id="1719a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1719a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1719a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1719a-123">Authorization</span></span>|<span data-ttu-id="1719a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1719a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1719a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1719a-125">Accept</span></span>|<span data-ttu-id="1719a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1719a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1719a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1719a-127">Request body</span></span>
<span data-ttu-id="1719a-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1719a-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

<span data-ttu-id="1719a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1719a-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md).</span></span>

|<span data-ttu-id="1719a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1719a-130">Property</span></span>|<span data-ttu-id="1719a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1719a-131">Type</span></span>|<span data-ttu-id="1719a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1719a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1719a-133">id</span><span class="sxs-lookup"><span data-stu-id="1719a-133">id</span></span>|<span data-ttu-id="1719a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1719a-134">String</span></span>|<span data-ttu-id="1719a-135">A chave para a política suplementar WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="1719a-135">The key for the WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="1719a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1719a-136">displayName</span></span>|<span data-ttu-id="1719a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1719a-137">String</span></span>|<span data-ttu-id="1719a-138">O nome de exibição da política suplementar WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="1719a-138">The display name of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="1719a-139">descrição</span><span class="sxs-lookup"><span data-stu-id="1719a-139">description</span></span>|<span data-ttu-id="1719a-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1719a-140">String</span></span>|<span data-ttu-id="1719a-141">A descrição da política suplementar WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="1719a-141">The description of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="1719a-142">conteúdo</span><span class="sxs-lookup"><span data-stu-id="1719a-142">content</span></span>|<span data-ttu-id="1719a-143">Binário</span><span class="sxs-lookup"><span data-stu-id="1719a-143">Binary</span></span>|<span data-ttu-id="1719a-144">O conteúdo da política suplementar WindowsDefenderApplicationControl no formato de matriz de byte.</span><span class="sxs-lookup"><span data-stu-id="1719a-144">The WindowsDefenderApplicationControl supplemental policy content in byte array format.</span></span>|
|<span data-ttu-id="1719a-145">contentFileName</span><span class="sxs-lookup"><span data-stu-id="1719a-145">contentFileName</span></span>|<span data-ttu-id="1719a-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1719a-146">String</span></span>|<span data-ttu-id="1719a-147">O nome do arquivo do conteúdo da política suplementar WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="1719a-147">The WindowsDefenderApplicationControl supplemental policy content's file name.</span></span>|
|<span data-ttu-id="1719a-148">versão</span><span class="sxs-lookup"><span data-stu-id="1719a-148">version</span></span>|<span data-ttu-id="1719a-149">String</span><span class="sxs-lookup"><span data-stu-id="1719a-149">String</span></span>|<span data-ttu-id="1719a-150">A versão da política suplementar WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="1719a-150">The WindowsDefenderApplicationControl supplemental policy's version.</span></span>|
|<span data-ttu-id="1719a-151">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="1719a-151">creationDateTime</span></span>|<span data-ttu-id="1719a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1719a-152">DateTimeOffset</span></span>|<span data-ttu-id="1719a-153">A data e a hora em que a política suplementar WindowsDefenderApplicationControl foi carregada.</span><span class="sxs-lookup"><span data-stu-id="1719a-153">The date and time when the WindowsDefenderApplicationControl supplemental policy was uploaded.</span></span>|
|<span data-ttu-id="1719a-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1719a-154">lastModifiedDateTime</span></span>|<span data-ttu-id="1719a-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1719a-155">DateTimeOffset</span></span>|<span data-ttu-id="1719a-156">A data e a hora em que a política suplementar WindowsDefenderApplicationControl foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1719a-156">The date and time when the WindowsDefenderApplicationControl supplemental policy was last modified.</span></span>|
|<span data-ttu-id="1719a-157">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1719a-157">roleScopeTagIds</span></span>|<span data-ttu-id="1719a-158">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1719a-158">String collection</span></span>|<span data-ttu-id="1719a-159">Lista de Marcas de Escopo para esta entidade de política suplementar WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="1719a-159">List of Scope Tags for this WindowsDefenderApplicationControl supplemental policy entity.</span></span>|



## <a name="response"></a><span data-ttu-id="1719a-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="1719a-160">Response</span></span>
<span data-ttu-id="1719a-161">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1719a-161">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1719a-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1719a-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="1719a-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1719a-163">Request</span></span>
<span data-ttu-id="1719a-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1719a-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
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

### <a name="response"></a><span data-ttu-id="1719a-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="1719a-165">Response</span></span>
<span data-ttu-id="1719a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1719a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




