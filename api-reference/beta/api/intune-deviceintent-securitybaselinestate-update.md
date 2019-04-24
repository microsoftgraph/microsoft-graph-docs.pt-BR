---
title: Atualizar securityBaselineState
description: Atualiza as propriedades de um objeto securityBaselineState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad0bca78fdf54054b9319853123ab0e79321ed59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466172"
---
# <a name="update-securitybaselinestate"></a><span data-ttu-id="ba732-103">Atualizar securityBaselineState</span><span class="sxs-lookup"><span data-stu-id="ba732-103">Update securityBaselineState</span></span>

> <span data-ttu-id="ba732-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ba732-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba732-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ba732-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba732-106">Atualiza as propriedades de um objeto [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) .</span><span class="sxs-lookup"><span data-stu-id="ba732-106">Update the properties of a [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba732-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ba732-107">Prerequisites</span></span>
<span data-ttu-id="ba732-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba732-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba732-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba732-110">Permission type</span></span>|<span data-ttu-id="ba732-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ba732-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba732-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba732-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba732-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba732-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ba732-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba732-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba732-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba732-115">Not supported.</span></span>|
|<span data-ttu-id="ba732-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba732-116">Application</span></span>|<span data-ttu-id="ba732-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba732-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba732-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba732-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}
```

## <a name="request-headers"></a><span data-ttu-id="ba732-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba732-119">Request headers</span></span>
|<span data-ttu-id="ba732-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba732-120">Header</span></span>|<span data-ttu-id="ba732-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ba732-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba732-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba732-122">Authorization</span></span>|<span data-ttu-id="ba732-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba732-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba732-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ba732-124">Accept</span></span>|<span data-ttu-id="ba732-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba732-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba732-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba732-126">Request body</span></span>
<span data-ttu-id="ba732-127">No corpo da solicitação, forneça uma representação JSON do objeto [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) .</span><span class="sxs-lookup"><span data-stu-id="ba732-127">In the request body, supply a JSON representation for the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>

<span data-ttu-id="ba732-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md).</span><span class="sxs-lookup"><span data-stu-id="ba732-128">The following table shows the properties that are required when you create the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md).</span></span>

|<span data-ttu-id="ba732-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba732-129">Property</span></span>|<span data-ttu-id="ba732-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba732-130">Type</span></span>|<span data-ttu-id="ba732-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba732-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba732-132">id</span><span class="sxs-lookup"><span data-stu-id="ba732-132">id</span></span>|<span data-ttu-id="ba732-133">String</span><span class="sxs-lookup"><span data-stu-id="ba732-133">String</span></span>|<span data-ttu-id="ba732-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ba732-134">Key of the entity.</span></span>|
|<span data-ttu-id="ba732-135">securityBaselineTemplateId</span><span class="sxs-lookup"><span data-stu-id="ba732-135">securityBaselineTemplateId</span></span>|<span data-ttu-id="ba732-136">String</span><span class="sxs-lookup"><span data-stu-id="ba732-136">String</span></span>|<span data-ttu-id="ba732-137">A ID do modelo de linha de base de segurança</span><span class="sxs-lookup"><span data-stu-id="ba732-137">The security baseline template id</span></span>|
|<span data-ttu-id="ba732-138">displayName</span><span class="sxs-lookup"><span data-stu-id="ba732-138">displayName</span></span>|<span data-ttu-id="ba732-139">String</span><span class="sxs-lookup"><span data-stu-id="ba732-139">String</span></span>|<span data-ttu-id="ba732-140">O nome de exibição da linha de base de segurança</span><span class="sxs-lookup"><span data-stu-id="ba732-140">The display name of the security baseline</span></span>|



## <a name="response"></a><span data-ttu-id="ba732-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba732-141">Response</span></span>
<span data-ttu-id="ba732-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba732-142">If successful, this method returns a `200 OK` response code and an updated [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba732-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba732-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba732-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba732-144">Request</span></span>
<span data-ttu-id="ba732-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba732-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}
Content-type: application/json
Content-length: 175

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="ba732-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba732-146">Response</span></span>
<span data-ttu-id="ba732-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba732-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 224

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "id": "23dc2503-2503-23dc-0325-dc230325dc23",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```



