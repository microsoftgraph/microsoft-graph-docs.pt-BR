---
title: Criar windowsDefenderApplicationControlSupplementalPolicy
description: Criar um novo objeto windowsDefenderApplicationControlSupplementalPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3ec672a7942e338297489a347f51532ffb42305a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457577"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicy"></a><span data-ttu-id="13807-103">Criar windowsDefenderApplicationControlSupplementalPolicy</span><span class="sxs-lookup"><span data-stu-id="13807-103">Create windowsDefenderApplicationControlSupplementalPolicy</span></span>

<span data-ttu-id="13807-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="13807-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13807-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="13807-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13807-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13807-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13807-107">Criar um novo objeto [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="13807-107">Create a new [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13807-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13807-108">Prerequisites</span></span>
<span data-ttu-id="13807-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13807-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13807-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13807-111">Permission type</span></span>|<span data-ttu-id="13807-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13807-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13807-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13807-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13807-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13807-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="13807-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13807-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13807-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13807-116">Not supported.</span></span>|
|<span data-ttu-id="13807-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13807-117">Application</span></span>|<span data-ttu-id="13807-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13807-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13807-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13807-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies
```

## <a name="request-headers"></a><span data-ttu-id="13807-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13807-120">Request headers</span></span>
|<span data-ttu-id="13807-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13807-121">Header</span></span>|<span data-ttu-id="13807-122">Valor</span><span class="sxs-lookup"><span data-stu-id="13807-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13807-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="13807-123">Authorization</span></span>|<span data-ttu-id="13807-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13807-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13807-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13807-125">Accept</span></span>|<span data-ttu-id="13807-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13807-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13807-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13807-127">Request body</span></span>
<span data-ttu-id="13807-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsDefenderApplicationControlSupplementalPolicy.</span><span class="sxs-lookup"><span data-stu-id="13807-128">In the request body, supply a JSON representation for the windowsDefenderApplicationControlSupplementalPolicy object.</span></span>

<span data-ttu-id="13807-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDefenderApplicationControlSupplementalPolicy.</span><span class="sxs-lookup"><span data-stu-id="13807-129">The following table shows the properties that are required when you create the windowsDefenderApplicationControlSupplementalPolicy.</span></span>

|<span data-ttu-id="13807-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13807-130">Property</span></span>|<span data-ttu-id="13807-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="13807-131">Type</span></span>|<span data-ttu-id="13807-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="13807-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13807-133">id</span><span class="sxs-lookup"><span data-stu-id="13807-133">id</span></span>|<span data-ttu-id="13807-134">String</span><span class="sxs-lookup"><span data-stu-id="13807-134">String</span></span>|<span data-ttu-id="13807-135">A chave da política complementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="13807-135">The key for the WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="13807-136">displayName</span><span class="sxs-lookup"><span data-stu-id="13807-136">displayName</span></span>|<span data-ttu-id="13807-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13807-137">String</span></span>|<span data-ttu-id="13807-138">O nome de exibição da política complementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="13807-138">The display name of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="13807-139">description</span><span class="sxs-lookup"><span data-stu-id="13807-139">description</span></span>|<span data-ttu-id="13807-140">String</span><span class="sxs-lookup"><span data-stu-id="13807-140">String</span></span>|<span data-ttu-id="13807-141">A descrição da política suplementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="13807-141">The description of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="13807-142">conteúdo</span><span class="sxs-lookup"><span data-stu-id="13807-142">content</span></span>|<span data-ttu-id="13807-143">Binária</span><span class="sxs-lookup"><span data-stu-id="13807-143">Binary</span></span>|<span data-ttu-id="13807-144">O conteúdo de política suplementar WindowsDefenderApplicationControl no formato de matriz de bytes.</span><span class="sxs-lookup"><span data-stu-id="13807-144">The WindowsDefenderApplicationControl supplemental policy content in byte array format.</span></span>|
|<span data-ttu-id="13807-145">contentFileName</span><span class="sxs-lookup"><span data-stu-id="13807-145">contentFileName</span></span>|<span data-ttu-id="13807-146">String</span><span class="sxs-lookup"><span data-stu-id="13807-146">String</span></span>|<span data-ttu-id="13807-147">O nome de arquivo do conteúdo da política suplementar da WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="13807-147">The WindowsDefenderApplicationControl supplemental policy content's file name.</span></span>|
|<span data-ttu-id="13807-148">versão</span><span class="sxs-lookup"><span data-stu-id="13807-148">version</span></span>|<span data-ttu-id="13807-149">String</span><span class="sxs-lookup"><span data-stu-id="13807-149">String</span></span>|<span data-ttu-id="13807-150">A versão da política suplementar da WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="13807-150">The WindowsDefenderApplicationControl supplemental policy's version.</span></span>|
|<span data-ttu-id="13807-151">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="13807-151">creationDateTime</span></span>|<span data-ttu-id="13807-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13807-152">DateTimeOffset</span></span>|<span data-ttu-id="13807-153">A data e a hora em que a política suplementar WindowsDefenderApplicationControl foi carregada.</span><span class="sxs-lookup"><span data-stu-id="13807-153">The date and time when the WindowsDefenderApplicationControl supplemental policy was uploaded.</span></span>|
|<span data-ttu-id="13807-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13807-154">lastModifiedDateTime</span></span>|<span data-ttu-id="13807-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13807-155">DateTimeOffset</span></span>|<span data-ttu-id="13807-156">A data e a hora da última modificação da política suplementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="13807-156">The date and time when the WindowsDefenderApplicationControl supplemental policy was last modified.</span></span>|
|<span data-ttu-id="13807-157">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="13807-157">roleScopeTagIds</span></span>|<span data-ttu-id="13807-158">String collection</span><span class="sxs-lookup"><span data-stu-id="13807-158">String collection</span></span>|<span data-ttu-id="13807-159">Lista de marcas de escopo para esta entidade de política suplementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="13807-159">List of Scope Tags for this WindowsDefenderApplicationControl supplemental policy entity.</span></span>|



## <a name="response"></a><span data-ttu-id="13807-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="13807-160">Response</span></span>
<span data-ttu-id="13807-161">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13807-161">If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13807-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13807-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="13807-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13807-163">Request</span></span>
<span data-ttu-id="13807-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13807-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="13807-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="13807-165">Response</span></span>
<span data-ttu-id="13807-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13807-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





