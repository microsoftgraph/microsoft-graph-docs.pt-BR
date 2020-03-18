---
title: Criar unsupportedGroupPolicyExtension
description: Criar um novo objeto unsupportedGroupPolicyExtension.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5a7826e00c2b0bccb6fa7e3832995fa67ea9dbd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804566"
---
# <a name="create-unsupportedgrouppolicyextension"></a><span data-ttu-id="0c3ec-103">Criar unsupportedGroupPolicyExtension</span><span class="sxs-lookup"><span data-stu-id="0c3ec-103">Create unsupportedGroupPolicyExtension</span></span>

> <span data-ttu-id="0c3ec-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0c3ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c3ec-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c3ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c3ec-106">Criar um novo objeto [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .</span><span class="sxs-lookup"><span data-stu-id="0c3ec-106">Create a new [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c3ec-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c3ec-107">Prerequisites</span></span>
<span data-ttu-id="0c3ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c3ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c3ec-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c3ec-110">Permission type</span></span>|<span data-ttu-id="0c3ec-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0c3ec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c3ec-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c3ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c3ec-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c3ec-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c3ec-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c3ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c3ec-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c3ec-115">Not supported.</span></span>|
|<span data-ttu-id="0c3ec-116">Application</span><span class="sxs-lookup"><span data-stu-id="0c3ec-116">Application</span></span>|<span data-ttu-id="0c3ec-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c3ec-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c3ec-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c3ec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
```

## <a name="request-headers"></a><span data-ttu-id="0c3ec-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c3ec-119">Request headers</span></span>
|<span data-ttu-id="0c3ec-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c3ec-120">Header</span></span>|<span data-ttu-id="0c3ec-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0c3ec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c3ec-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c3ec-122">Authorization</span></span>|<span data-ttu-id="0c3ec-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c3ec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c3ec-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c3ec-124">Accept</span></span>|<span data-ttu-id="0c3ec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c3ec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c3ec-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c3ec-126">Request body</span></span>
<span data-ttu-id="0c3ec-127">No corpo da solicitação, forneça uma representação JSON do objeto unsupportedGroupPolicyExtension.</span><span class="sxs-lookup"><span data-stu-id="0c3ec-127">In the request body, supply a JSON representation for the unsupportedGroupPolicyExtension object.</span></span>

<span data-ttu-id="0c3ec-128">A tabela a seguir mostra as propriedades que são necessárias ao criar unsupportedGroupPolicyExtension.</span><span class="sxs-lookup"><span data-stu-id="0c3ec-128">The following table shows the properties that are required when you create the unsupportedGroupPolicyExtension.</span></span>

|<span data-ttu-id="0c3ec-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c3ec-129">Property</span></span>|<span data-ttu-id="0c3ec-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c3ec-130">Type</span></span>|<span data-ttu-id="0c3ec-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c3ec-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c3ec-132">id</span><span class="sxs-lookup"><span data-stu-id="0c3ec-132">id</span></span>|<span data-ttu-id="0c3ec-133">String</span><span class="sxs-lookup"><span data-stu-id="0c3ec-133">String</span></span>|<span data-ttu-id="0c3ec-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0c3ec-134">Not yet documented</span></span>|
|<span data-ttu-id="0c3ec-135">settingScope</span><span class="sxs-lookup"><span data-stu-id="0c3ec-135">settingScope</span></span>|[<span data-ttu-id="0c3ec-136">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="0c3ec-136">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="0c3ec-137">Definindo o escopo da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c3ec-137">Setting Scope of the unsupported extension.</span></span> <span data-ttu-id="0c3ec-138">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="0c3ec-138">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="0c3ec-139">namespaceUrl</span><span class="sxs-lookup"><span data-stu-id="0c3ec-139">namespaceUrl</span></span>|<span data-ttu-id="0c3ec-140">String</span><span class="sxs-lookup"><span data-stu-id="0c3ec-140">String</span></span>|<span data-ttu-id="0c3ec-141">URL do namespace da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c3ec-141">Namespace Url of the unsupported extension.</span></span>|
|<span data-ttu-id="0c3ec-142">ExtensionType</span><span class="sxs-lookup"><span data-stu-id="0c3ec-142">extensionType</span></span>|<span data-ttu-id="0c3ec-143">String</span><span class="sxs-lookup"><span data-stu-id="0c3ec-143">String</span></span>|<span data-ttu-id="0c3ec-144">ExtensionType da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c3ec-144">ExtensionType of the unsupported extension.</span></span>|
|<span data-ttu-id="0c3ec-145">Nome</span><span class="sxs-lookup"><span data-stu-id="0c3ec-145">nodeName</span></span>|<span data-ttu-id="0c3ec-146">String</span><span class="sxs-lookup"><span data-stu-id="0c3ec-146">String</span></span>|<span data-ttu-id="0c3ec-147">Nome do nó da extensão sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c3ec-147">Node name of the unsupported extension.</span></span>|



## <a name="response"></a><span data-ttu-id="0c3ec-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c3ec-148">Response</span></span>
<span data-ttu-id="0c3ec-149">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c3ec-149">If successful, this method returns a `201 Created` response code and a [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c3ec-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c3ec-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c3ec-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c3ec-151">Request</span></span>
<span data-ttu-id="0c3ec-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c3ec-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0c3ec-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c3ec-153">Response</span></span>
<span data-ttu-id="0c3ec-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c3ec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




