---
title: Criar unsupportedGroupPolicyExtension
description: Crie um novo objeto UnsupportedGroupPolicyExtension.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ccee92daa5d468dcebebd59acaa764bd65297195
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149818"
---
# <a name="create-unsupportedgrouppolicyextension"></a><span data-ttu-id="e9682-103">Criar unsupportedGroupPolicyExtension</span><span class="sxs-lookup"><span data-stu-id="e9682-103">Create unsupportedGroupPolicyExtension</span></span>

<span data-ttu-id="e9682-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9682-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9682-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e9682-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9682-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9682-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9682-107">Crie um novo [objeto UnsupportedGroupPolicyExtension.](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)</span><span class="sxs-lookup"><span data-stu-id="e9682-107">Create a new [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9682-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e9682-108">Prerequisites</span></span>
<span data-ttu-id="e9682-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9682-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9682-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9682-111">Permission type</span></span>|<span data-ttu-id="e9682-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9682-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9682-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9682-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9682-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9682-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e9682-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9682-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9682-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9682-116">Not supported.</span></span>|
|<span data-ttu-id="e9682-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9682-117">Application</span></span>|<span data-ttu-id="e9682-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9682-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9682-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9682-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
```

## <a name="request-headers"></a><span data-ttu-id="e9682-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9682-120">Request headers</span></span>
|<span data-ttu-id="e9682-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9682-121">Header</span></span>|<span data-ttu-id="e9682-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e9682-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9682-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9682-123">Authorization</span></span>|<span data-ttu-id="e9682-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9682-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9682-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e9682-125">Accept</span></span>|<span data-ttu-id="e9682-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9682-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9682-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9682-127">Request body</span></span>
<span data-ttu-id="e9682-128">No corpo da solicitação, fornece uma representação JSON para o objeto UnsupportedGroupPolicyExtension.</span><span class="sxs-lookup"><span data-stu-id="e9682-128">In the request body, supply a JSON representation for the unsupportedGroupPolicyExtension object.</span></span>

<span data-ttu-id="e9682-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o UnsupportedGroupPolicyExtension.</span><span class="sxs-lookup"><span data-stu-id="e9682-129">The following table shows the properties that are required when you create the unsupportedGroupPolicyExtension.</span></span>

|<span data-ttu-id="e9682-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9682-130">Property</span></span>|<span data-ttu-id="e9682-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9682-131">Type</span></span>|<span data-ttu-id="e9682-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9682-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9682-133">id</span><span class="sxs-lookup"><span data-stu-id="e9682-133">id</span></span>|<span data-ttu-id="e9682-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9682-134">String</span></span>|<span data-ttu-id="e9682-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e9682-135">Not yet documented</span></span>|
|<span data-ttu-id="e9682-136">settingScope</span><span class="sxs-lookup"><span data-stu-id="e9682-136">settingScope</span></span>|[<span data-ttu-id="e9682-137">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="e9682-137">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="e9682-138">Definindo Escopo da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9682-138">Setting Scope of the unsupported extension.</span></span> <span data-ttu-id="e9682-139">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="e9682-139">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="e9682-140">namespaceUrl</span><span class="sxs-lookup"><span data-stu-id="e9682-140">namespaceUrl</span></span>|<span data-ttu-id="e9682-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9682-141">String</span></span>|<span data-ttu-id="e9682-142">Url do namespace da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9682-142">Namespace Url of the unsupported extension.</span></span>|
|<span data-ttu-id="e9682-143">extensionType</span><span class="sxs-lookup"><span data-stu-id="e9682-143">extensionType</span></span>|<span data-ttu-id="e9682-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9682-144">String</span></span>|<span data-ttu-id="e9682-145">ExtensionType da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9682-145">ExtensionType of the unsupported extension.</span></span>|
|<span data-ttu-id="e9682-146">nodeName</span><span class="sxs-lookup"><span data-stu-id="e9682-146">nodeName</span></span>|<span data-ttu-id="e9682-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9682-147">String</span></span>|<span data-ttu-id="e9682-148">Nome do nó da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9682-148">Node name of the unsupported extension.</span></span>|



## <a name="response"></a><span data-ttu-id="e9682-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9682-149">Response</span></span>
<span data-ttu-id="e9682-150">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto UnsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9682-150">If successful, this method returns a `201 Created` response code and a [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9682-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9682-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9682-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9682-152">Request</span></span>
<span data-ttu-id="e9682-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9682-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
  "settingScope": "device",
  "namespaceUrl": "https://example.com/namespaceUrl/",
  "extensionType": "Extension Type value",
  "nodeName": "Node Name value"
}
```

### <a name="response"></a><span data-ttu-id="e9682-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9682-154">Response</span></span>
<span data-ttu-id="e9682-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9682-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
  "id": "e59ecce2-cce2-e59e-e2cc-9ee5e2cc9ee5",
  "settingScope": "device",
  "namespaceUrl": "https://example.com/namespaceUrl/",
  "extensionType": "Extension Type value",
  "nodeName": "Node Name value"
}
```




