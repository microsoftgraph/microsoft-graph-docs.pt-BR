---
title: Atualizar unsupportedGroupPolicyExtension
description: Atualiza as propriedades de um objeto unsupportedGroupPolicyExtension.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b4e7d5656d78178a445d98c789d70246919ee07
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804538"
---
# <a name="update-unsupportedgrouppolicyextension"></a><span data-ttu-id="e9500-103">Atualizar unsupportedGroupPolicyExtension</span><span class="sxs-lookup"><span data-stu-id="e9500-103">Update unsupportedGroupPolicyExtension</span></span>

> <span data-ttu-id="e9500-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e9500-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9500-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9500-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9500-106">Atualiza as propriedades de um objeto [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .</span><span class="sxs-lookup"><span data-stu-id="e9500-106">Update the properties of a [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9500-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e9500-107">Prerequisites</span></span>
<span data-ttu-id="e9500-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9500-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9500-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9500-110">Permission type</span></span>|<span data-ttu-id="e9500-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e9500-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9500-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9500-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e9500-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9500-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e9500-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9500-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9500-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9500-115">Not supported.</span></span>|
|<span data-ttu-id="e9500-116">Application</span><span class="sxs-lookup"><span data-stu-id="e9500-116">Application</span></span>|<span data-ttu-id="e9500-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9500-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9500-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9500-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions/{unsupportedGroupPolicyExtensionId}
```

## <a name="request-headers"></a><span data-ttu-id="e9500-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9500-119">Request headers</span></span>
|<span data-ttu-id="e9500-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9500-120">Header</span></span>|<span data-ttu-id="e9500-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e9500-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9500-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9500-122">Authorization</span></span>|<span data-ttu-id="e9500-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9500-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9500-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e9500-124">Accept</span></span>|<span data-ttu-id="e9500-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e9500-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9500-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9500-126">Request body</span></span>
<span data-ttu-id="e9500-127">No corpo da solicitação, forneça uma representação JSON do objeto [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .</span><span class="sxs-lookup"><span data-stu-id="e9500-127">In the request body, supply a JSON representation for the [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

<span data-ttu-id="e9500-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md).</span><span class="sxs-lookup"><span data-stu-id="e9500-128">The following table shows the properties that are required when you create the [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md).</span></span>

|<span data-ttu-id="e9500-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9500-129">Property</span></span>|<span data-ttu-id="e9500-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9500-130">Type</span></span>|<span data-ttu-id="e9500-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9500-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9500-132">id</span><span class="sxs-lookup"><span data-stu-id="e9500-132">id</span></span>|<span data-ttu-id="e9500-133">String</span><span class="sxs-lookup"><span data-stu-id="e9500-133">String</span></span>|<span data-ttu-id="e9500-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e9500-134">Not yet documented</span></span>|
|<span data-ttu-id="e9500-135">settingScope</span><span class="sxs-lookup"><span data-stu-id="e9500-135">settingScope</span></span>|[<span data-ttu-id="e9500-136">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="e9500-136">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="e9500-137">Definindo o escopo da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9500-137">Setting Scope of the unsupported extension.</span></span> <span data-ttu-id="e9500-138">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="e9500-138">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="e9500-139">namespaceUrl</span><span class="sxs-lookup"><span data-stu-id="e9500-139">namespaceUrl</span></span>|<span data-ttu-id="e9500-140">String</span><span class="sxs-lookup"><span data-stu-id="e9500-140">String</span></span>|<span data-ttu-id="e9500-141">URL do namespace da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9500-141">Namespace Url of the unsupported extension.</span></span>|
|<span data-ttu-id="e9500-142">ExtensionType</span><span class="sxs-lookup"><span data-stu-id="e9500-142">extensionType</span></span>|<span data-ttu-id="e9500-143">String</span><span class="sxs-lookup"><span data-stu-id="e9500-143">String</span></span>|<span data-ttu-id="e9500-144">ExtensionType da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9500-144">ExtensionType of the unsupported extension.</span></span>|
|<span data-ttu-id="e9500-145">Nome</span><span class="sxs-lookup"><span data-stu-id="e9500-145">nodeName</span></span>|<span data-ttu-id="e9500-146">String</span><span class="sxs-lookup"><span data-stu-id="e9500-146">String</span></span>|<span data-ttu-id="e9500-147">Nome do nó da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9500-147">Node name of the unsupported extension.</span></span>|



## <a name="response"></a><span data-ttu-id="e9500-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9500-148">Response</span></span>
<span data-ttu-id="e9500-149">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9500-149">If successful, this method returns a `200 OK` response code and an updated [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9500-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9500-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9500-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9500-151">Request</span></span>
<span data-ttu-id="e9500-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9500-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions/{unsupportedGroupPolicyExtensionId}
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

### <a name="response"></a><span data-ttu-id="e9500-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9500-153">Response</span></span>
<span data-ttu-id="e9500-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9500-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




