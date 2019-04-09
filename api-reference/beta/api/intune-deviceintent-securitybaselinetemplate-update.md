---
title: Atualizar securityBaselineTemplate
description: Atualiza as propriedades de um objeto securityBaselineTemplate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8d407646c4369352d8ce8f1760c5a64f4d99dbc
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522766"
---
# <a name="update-securitybaselinetemplate"></a><span data-ttu-id="ae264-103">Atualizar securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="ae264-103">Update securityBaselineTemplate</span></span>

> <span data-ttu-id="ae264-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae264-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae264-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae264-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae264-106">Atualiza as propriedades de um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="ae264-106">Update the properties of a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae264-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae264-107">Prerequisites</span></span>
<span data-ttu-id="ae264-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae264-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae264-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae264-110">Permission type</span></span>|<span data-ttu-id="ae264-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ae264-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae264-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae264-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae264-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae264-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae264-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae264-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae264-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae264-115">Not supported.</span></span>|
|<span data-ttu-id="ae264-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae264-116">Application</span></span>|<span data-ttu-id="ae264-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae264-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae264-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae264-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="ae264-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae264-119">Request headers</span></span>
|<span data-ttu-id="ae264-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae264-120">Header</span></span>|<span data-ttu-id="ae264-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ae264-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae264-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae264-122">Authorization</span></span>|<span data-ttu-id="ae264-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae264-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae264-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae264-124">Accept</span></span>|<span data-ttu-id="ae264-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae264-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae264-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae264-126">Request body</span></span>
<span data-ttu-id="ae264-127">No corpo da solicitação, forneça uma representação JSON do objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="ae264-127">In the request body, supply a JSON representation for the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

<span data-ttu-id="ae264-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="ae264-128">The following table shows the properties that are required when you create the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span></span>

|<span data-ttu-id="ae264-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae264-129">Property</span></span>|<span data-ttu-id="ae264-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae264-130">Type</span></span>|<span data-ttu-id="ae264-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae264-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae264-132">id</span><span class="sxs-lookup"><span data-stu-id="ae264-132">id</span></span>|<span data-ttu-id="ae264-133">String</span><span class="sxs-lookup"><span data-stu-id="ae264-133">String</span></span>|<span data-ttu-id="ae264-134">A ID do modelo herdada de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="ae264-134">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="ae264-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ae264-135">displayName</span></span>|<span data-ttu-id="ae264-136">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="ae264-136">String</span></span>|<span data-ttu-id="ae264-137">O nome de exibição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="ae264-137">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="ae264-138">description</span><span class="sxs-lookup"><span data-stu-id="ae264-138">description</span></span>|<span data-ttu-id="ae264-139">String</span><span class="sxs-lookup"><span data-stu-id="ae264-139">String</span></span>|<span data-ttu-id="ae264-140">A descrição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="ae264-140">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ae264-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae264-141">Response</span></span>
<span data-ttu-id="ae264-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae264-142">If successful, this method returns a `200 OK` response code and an updated [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae264-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae264-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae264-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae264-144">Request</span></span>
<span data-ttu-id="ae264-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae264-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="ae264-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae264-146">Response</span></span>
<span data-ttu-id="ae264-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae264-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 194

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value"
}
```







