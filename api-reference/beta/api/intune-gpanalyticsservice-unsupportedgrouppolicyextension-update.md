---
title: Atualizar unsupportedGroupPolicyExtension
description: Atualiza as propriedades de um objeto unsupportedGroupPolicyExtension.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d3b7eda504ee8cc3382427dbe352b2b73e7f836a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49286007"
---
# <a name="update-unsupportedgrouppolicyextension"></a><span data-ttu-id="48dac-103">Atualizar unsupportedGroupPolicyExtension</span><span class="sxs-lookup"><span data-stu-id="48dac-103">Update unsupportedGroupPolicyExtension</span></span>

<span data-ttu-id="48dac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48dac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48dac-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48dac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48dac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48dac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48dac-107">Atualiza as propriedades de um objeto [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .</span><span class="sxs-lookup"><span data-stu-id="48dac-107">Update the properties of a [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48dac-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="48dac-108">Prerequisites</span></span>
<span data-ttu-id="48dac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48dac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48dac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48dac-111">Permission type</span></span>|<span data-ttu-id="48dac-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="48dac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48dac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48dac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48dac-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48dac-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="48dac-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48dac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48dac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48dac-116">Not supported.</span></span>|
|<span data-ttu-id="48dac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48dac-117">Application</span></span>|<span data-ttu-id="48dac-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48dac-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48dac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48dac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions/{unsupportedGroupPolicyExtensionId}
```

## <a name="request-headers"></a><span data-ttu-id="48dac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48dac-120">Request headers</span></span>
|<span data-ttu-id="48dac-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="48dac-121">Header</span></span>|<span data-ttu-id="48dac-122">Valor</span><span class="sxs-lookup"><span data-stu-id="48dac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48dac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="48dac-123">Authorization</span></span>|<span data-ttu-id="48dac-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48dac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48dac-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="48dac-125">Accept</span></span>|<span data-ttu-id="48dac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48dac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48dac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48dac-127">Request body</span></span>
<span data-ttu-id="48dac-128">No corpo da solicitação, forneça uma representação JSON do objeto [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .</span><span class="sxs-lookup"><span data-stu-id="48dac-128">In the request body, supply a JSON representation for the [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

<span data-ttu-id="48dac-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md).</span><span class="sxs-lookup"><span data-stu-id="48dac-129">The following table shows the properties that are required when you create the [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md).</span></span>

|<span data-ttu-id="48dac-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48dac-130">Property</span></span>|<span data-ttu-id="48dac-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="48dac-131">Type</span></span>|<span data-ttu-id="48dac-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="48dac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48dac-133">id</span><span class="sxs-lookup"><span data-stu-id="48dac-133">id</span></span>|<span data-ttu-id="48dac-134">String</span><span class="sxs-lookup"><span data-stu-id="48dac-134">String</span></span>|<span data-ttu-id="48dac-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48dac-135">Not yet documented</span></span>|
|<span data-ttu-id="48dac-136">settingScope</span><span class="sxs-lookup"><span data-stu-id="48dac-136">settingScope</span></span>|[<span data-ttu-id="48dac-137">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="48dac-137">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="48dac-138">Definindo o escopo da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48dac-138">Setting Scope of the unsupported extension.</span></span> <span data-ttu-id="48dac-139">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="48dac-139">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="48dac-140">namespaceUrl</span><span class="sxs-lookup"><span data-stu-id="48dac-140">namespaceUrl</span></span>|<span data-ttu-id="48dac-141">String</span><span class="sxs-lookup"><span data-stu-id="48dac-141">String</span></span>|<span data-ttu-id="48dac-142">URL do namespace da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48dac-142">Namespace Url of the unsupported extension.</span></span>|
|<span data-ttu-id="48dac-143">ExtensionType</span><span class="sxs-lookup"><span data-stu-id="48dac-143">extensionType</span></span>|<span data-ttu-id="48dac-144">String</span><span class="sxs-lookup"><span data-stu-id="48dac-144">String</span></span>|<span data-ttu-id="48dac-145">ExtensionType da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48dac-145">ExtensionType of the unsupported extension.</span></span>|
|<span data-ttu-id="48dac-146">Nome</span><span class="sxs-lookup"><span data-stu-id="48dac-146">nodeName</span></span>|<span data-ttu-id="48dac-147">String</span><span class="sxs-lookup"><span data-stu-id="48dac-147">String</span></span>|<span data-ttu-id="48dac-148">Nome do nó da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48dac-148">Node name of the unsupported extension.</span></span>|



## <a name="response"></a><span data-ttu-id="48dac-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="48dac-149">Response</span></span>
<span data-ttu-id="48dac-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48dac-150">If successful, this method returns a `200 OK` response code and an updated [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48dac-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48dac-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="48dac-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48dac-152">Request</span></span>
<span data-ttu-id="48dac-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48dac-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="48dac-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="48dac-154">Response</span></span>
<span data-ttu-id="48dac-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48dac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




