---
title: Criar unsupportedGroupPolicyExtension
description: Criar um novo objeto unsupportedGroupPolicyExtension.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4527a57e68325e18634587661f1a15634ec8c75a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074556"
---
# <a name="create-unsupportedgrouppolicyextension"></a><span data-ttu-id="fb7e8-103">Criar unsupportedGroupPolicyExtension</span><span class="sxs-lookup"><span data-stu-id="fb7e8-103">Create unsupportedGroupPolicyExtension</span></span>

<span data-ttu-id="fb7e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb7e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb7e8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fb7e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb7e8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb7e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb7e8-107">Criar um novo objeto [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .</span><span class="sxs-lookup"><span data-stu-id="fb7e8-107">Create a new [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb7e8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fb7e8-108">Prerequisites</span></span>
<span data-ttu-id="fb7e8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb7e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb7e8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb7e8-111">Permission type</span></span>|<span data-ttu-id="fb7e8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fb7e8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb7e8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb7e8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb7e8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb7e8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb7e8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb7e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb7e8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb7e8-116">Not supported.</span></span>|
|<span data-ttu-id="fb7e8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb7e8-117">Application</span></span>|<span data-ttu-id="fb7e8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb7e8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb7e8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb7e8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
```

## <a name="request-headers"></a><span data-ttu-id="fb7e8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb7e8-120">Request headers</span></span>
|<span data-ttu-id="fb7e8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb7e8-121">Header</span></span>|<span data-ttu-id="fb7e8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fb7e8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb7e8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb7e8-123">Authorization</span></span>|<span data-ttu-id="fb7e8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb7e8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb7e8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fb7e8-125">Accept</span></span>|<span data-ttu-id="fb7e8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb7e8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb7e8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb7e8-127">Request body</span></span>
<span data-ttu-id="fb7e8-128">No corpo da solicitação, forneça uma representação JSON do objeto unsupportedGroupPolicyExtension.</span><span class="sxs-lookup"><span data-stu-id="fb7e8-128">In the request body, supply a JSON representation for the unsupportedGroupPolicyExtension object.</span></span>

<span data-ttu-id="fb7e8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar unsupportedGroupPolicyExtension.</span><span class="sxs-lookup"><span data-stu-id="fb7e8-129">The following table shows the properties that are required when you create the unsupportedGroupPolicyExtension.</span></span>

|<span data-ttu-id="fb7e8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb7e8-130">Property</span></span>|<span data-ttu-id="fb7e8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb7e8-131">Type</span></span>|<span data-ttu-id="fb7e8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb7e8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb7e8-133">id</span><span class="sxs-lookup"><span data-stu-id="fb7e8-133">id</span></span>|<span data-ttu-id="fb7e8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb7e8-134">String</span></span>|<span data-ttu-id="fb7e8-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fb7e8-135">Not yet documented</span></span>|
|<span data-ttu-id="fb7e8-136">settingScope</span><span class="sxs-lookup"><span data-stu-id="fb7e8-136">settingScope</span></span>|[<span data-ttu-id="fb7e8-137">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="fb7e8-137">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="fb7e8-138">Definindo o escopo da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb7e8-138">Setting Scope of the unsupported extension.</span></span> <span data-ttu-id="fb7e8-139">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="fb7e8-139">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="fb7e8-140">namespaceUrl</span><span class="sxs-lookup"><span data-stu-id="fb7e8-140">namespaceUrl</span></span>|<span data-ttu-id="fb7e8-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb7e8-141">String</span></span>|<span data-ttu-id="fb7e8-142">URL do namespace da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb7e8-142">Namespace Url of the unsupported extension.</span></span>|
|<span data-ttu-id="fb7e8-143">ExtensionType</span><span class="sxs-lookup"><span data-stu-id="fb7e8-143">extensionType</span></span>|<span data-ttu-id="fb7e8-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb7e8-144">String</span></span>|<span data-ttu-id="fb7e8-145">ExtensionType da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb7e8-145">ExtensionType of the unsupported extension.</span></span>|
|<span data-ttu-id="fb7e8-146">Nome</span><span class="sxs-lookup"><span data-stu-id="fb7e8-146">nodeName</span></span>|<span data-ttu-id="fb7e8-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb7e8-147">String</span></span>|<span data-ttu-id="fb7e8-148">Nome do nó da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb7e8-148">Node name of the unsupported extension.</span></span>|



## <a name="response"></a><span data-ttu-id="fb7e8-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb7e8-149">Response</span></span>
<span data-ttu-id="fb7e8-150">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb7e8-150">If successful, this method returns a `201 Created` response code and a [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb7e8-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb7e8-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb7e8-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb7e8-152">Request</span></span>
<span data-ttu-id="fb7e8-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb7e8-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fb7e8-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb7e8-154">Response</span></span>
<span data-ttu-id="fb7e8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb7e8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






