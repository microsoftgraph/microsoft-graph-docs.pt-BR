---
title: Criar securityBaselineTemplate
description: Criar um novo objeto securityBaselineTemplate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d6f48f0fdb95f2d88f6af5f62975792453367d9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773487"
---
# <a name="create-securitybaselinetemplate"></a><span data-ttu-id="1ab21-103">Criar securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="1ab21-103">Create securityBaselineTemplate</span></span>

> <span data-ttu-id="1ab21-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ab21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ab21-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ab21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ab21-106">Criar um novo objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="1ab21-106">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ab21-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1ab21-107">Prerequisites</span></span>
<span data-ttu-id="1ab21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ab21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ab21-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ab21-110">Permission type</span></span>|<span data-ttu-id="1ab21-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1ab21-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ab21-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ab21-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ab21-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ab21-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1ab21-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ab21-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ab21-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ab21-115">Not supported.</span></span>|
|<span data-ttu-id="1ab21-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ab21-116">Application</span></span>|<span data-ttu-id="1ab21-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ab21-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ab21-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ab21-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
```

## <a name="request-headers"></a><span data-ttu-id="1ab21-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ab21-119">Request headers</span></span>
|<span data-ttu-id="1ab21-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1ab21-120">Header</span></span>|<span data-ttu-id="1ab21-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1ab21-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ab21-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ab21-122">Authorization</span></span>|<span data-ttu-id="1ab21-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ab21-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ab21-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1ab21-124">Accept</span></span>|<span data-ttu-id="1ab21-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1ab21-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ab21-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ab21-126">Request body</span></span>
<span data-ttu-id="1ab21-127">No corpo da solicitação, forneça uma representação JSON do objeto securityBaselineTemplate.</span><span class="sxs-lookup"><span data-stu-id="1ab21-127">In the request body, supply a JSON representation for the securityBaselineTemplate object.</span></span>

<span data-ttu-id="1ab21-128">A tabela a seguir mostra as propriedades que são necessárias ao criar securityBaselineTemplate.</span><span class="sxs-lookup"><span data-stu-id="1ab21-128">The following table shows the properties that are required when you create the securityBaselineTemplate.</span></span>

|<span data-ttu-id="1ab21-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ab21-129">Property</span></span>|<span data-ttu-id="1ab21-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ab21-130">Type</span></span>|<span data-ttu-id="1ab21-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ab21-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ab21-132">id</span><span class="sxs-lookup"><span data-stu-id="1ab21-132">id</span></span>|<span data-ttu-id="1ab21-133">String</span><span class="sxs-lookup"><span data-stu-id="1ab21-133">String</span></span>|<span data-ttu-id="1ab21-134">A ID do modelo herdada de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="1ab21-134">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="1ab21-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1ab21-135">displayName</span></span>|<span data-ttu-id="1ab21-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ab21-136">String</span></span>|<span data-ttu-id="1ab21-137">O nome de exibição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="1ab21-137">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="1ab21-138">description</span><span class="sxs-lookup"><span data-stu-id="1ab21-138">description</span></span>|<span data-ttu-id="1ab21-139">String</span><span class="sxs-lookup"><span data-stu-id="1ab21-139">String</span></span>|<span data-ttu-id="1ab21-140">A descrição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="1ab21-140">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1ab21-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ab21-141">Response</span></span>
<span data-ttu-id="1ab21-142">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ab21-142">If successful, this method returns a `201 Created` response code and a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ab21-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ab21-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ab21-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ab21-144">Request</span></span>
<span data-ttu-id="1ab21-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ab21-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="1ab21-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ab21-146">Response</span></span>
<span data-ttu-id="1ab21-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ab21-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 194

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value"
}
```





