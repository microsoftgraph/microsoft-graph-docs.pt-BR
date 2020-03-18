---
title: Excluir deviceComplianceUserStatus
description: Exclui deviceComplianceUserStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f4ecf10f8cae97a5779da85169110ebd6d5908ba
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42754836"
---
# <a name="delete-devicecomplianceuserstatus"></a><span data-ttu-id="13f52-103">Excluir deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="13f52-103">Delete deviceComplianceUserStatus</span></span>

> <span data-ttu-id="13f52-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="13f52-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13f52-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13f52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13f52-106">Exclui [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="13f52-106">Deletes a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13f52-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13f52-107">Prerequisites</span></span>
<span data-ttu-id="13f52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13f52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13f52-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13f52-110">Permission type</span></span>|<span data-ttu-id="13f52-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13f52-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13f52-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13f52-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13f52-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13f52-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="13f52-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13f52-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13f52-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13f52-115">Not supported.</span></span>|
|<span data-ttu-id="13f52-116">Application</span><span class="sxs-lookup"><span data-stu-id="13f52-116">Application</span></span>|<span data-ttu-id="13f52-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13f52-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13f52-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13f52-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="13f52-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13f52-119">Request headers</span></span>
|<span data-ttu-id="13f52-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13f52-120">Header</span></span>|<span data-ttu-id="13f52-121">Valor</span><span class="sxs-lookup"><span data-stu-id="13f52-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13f52-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="13f52-122">Authorization</span></span>|<span data-ttu-id="13f52-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13f52-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13f52-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13f52-124">Accept</span></span>|<span data-ttu-id="13f52-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13f52-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13f52-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13f52-126">Request body</span></span>
<span data-ttu-id="13f52-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13f52-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13f52-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="13f52-128">Response</span></span>
<span data-ttu-id="13f52-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="13f52-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="13f52-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13f52-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="13f52-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13f52-131">Request</span></span>
<span data-ttu-id="13f52-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13f52-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

### <a name="response"></a><span data-ttu-id="13f52-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="13f52-133">Response</span></span>
<span data-ttu-id="13f52-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13f52-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




