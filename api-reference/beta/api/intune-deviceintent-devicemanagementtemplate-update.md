---
title: Atualizar deviceManagementTemplate
description: Atualiza as propriedades de um objeto deviceManagementTemplate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e19114de1b10f3c3bf9a9e237eebac3a1103172a
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523613"
---
# <a name="update-devicemanagementtemplate"></a><span data-ttu-id="b2d3e-103">Atualizar deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="b2d3e-103">Update deviceManagementTemplate</span></span>

> <span data-ttu-id="b2d3e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2d3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2d3e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2d3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2d3e-106">Atualiza as propriedades de um objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="b2d3e-106">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2d3e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2d3e-107">Prerequisites</span></span>
<span data-ttu-id="b2d3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2d3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2d3e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2d3e-110">Permission type</span></span>|<span data-ttu-id="b2d3e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2d3e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2d3e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2d3e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2d3e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2d3e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2d3e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2d3e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2d3e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2d3e-115">Not supported.</span></span>|
|<span data-ttu-id="b2d3e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2d3e-116">Application</span></span>|<span data-ttu-id="b2d3e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2d3e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2d3e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2d3e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="b2d3e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d3e-119">Request headers</span></span>
|<span data-ttu-id="b2d3e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2d3e-120">Header</span></span>|<span data-ttu-id="b2d3e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b2d3e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2d3e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2d3e-122">Authorization</span></span>|<span data-ttu-id="b2d3e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2d3e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2d3e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2d3e-124">Accept</span></span>|<span data-ttu-id="b2d3e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2d3e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2d3e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d3e-126">Request body</span></span>
<span data-ttu-id="b2d3e-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="b2d3e-127">In the request body, supply a JSON representation for the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

<span data-ttu-id="b2d3e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="b2d3e-128">The following table shows the properties that are required when you create the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>

|<span data-ttu-id="b2d3e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2d3e-129">Property</span></span>|<span data-ttu-id="b2d3e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2d3e-130">Type</span></span>|<span data-ttu-id="b2d3e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2d3e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2d3e-132">id</span><span class="sxs-lookup"><span data-stu-id="b2d3e-132">id</span></span>|<span data-ttu-id="b2d3e-133">String</span><span class="sxs-lookup"><span data-stu-id="b2d3e-133">String</span></span>|<span data-ttu-id="b2d3e-134">A ID do modelo</span><span class="sxs-lookup"><span data-stu-id="b2d3e-134">The template ID</span></span>|
|<span data-ttu-id="b2d3e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b2d3e-135">displayName</span></span>|<span data-ttu-id="b2d3e-136">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b2d3e-136">String</span></span>|<span data-ttu-id="b2d3e-137">O nome de exibição do modelo</span><span class="sxs-lookup"><span data-stu-id="b2d3e-137">The template's display name</span></span>|
|<span data-ttu-id="b2d3e-138">description</span><span class="sxs-lookup"><span data-stu-id="b2d3e-138">description</span></span>|<span data-ttu-id="b2d3e-139">String</span><span class="sxs-lookup"><span data-stu-id="b2d3e-139">String</span></span>|<span data-ttu-id="b2d3e-140">A descrição do modelo</span><span class="sxs-lookup"><span data-stu-id="b2d3e-140">The template's description</span></span>|



## <a name="response"></a><span data-ttu-id="b2d3e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2d3e-141">Response</span></span>
<span data-ttu-id="b2d3e-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2d3e-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2d3e-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2d3e-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2d3e-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d3e-144">Request</span></span>
<span data-ttu-id="b2d3e-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2d3e-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="b2d3e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2d3e-146">Response</span></span>
<span data-ttu-id="b2d3e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2d3e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 194

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
  "displayName": "Display Name value",
  "description": "Description value"
}
```







