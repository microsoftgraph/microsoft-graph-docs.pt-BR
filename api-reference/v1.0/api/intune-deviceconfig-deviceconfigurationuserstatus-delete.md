---
title: Excluir deviceConfigurationUserStatus
description: Exclui deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 49121b6ea9ed026ba1aa3a1d080620867cb0fffc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066835"
---
# <a name="delete-deviceconfigurationuserstatus"></a><span data-ttu-id="342dc-103">Excluir deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="342dc-103">Delete deviceConfigurationUserStatus</span></span>

<span data-ttu-id="342dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="342dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="342dc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="342dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="342dc-106">Exclui [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="342dc-106">Deletes a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="342dc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="342dc-107">Prerequisites</span></span>
<span data-ttu-id="342dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="342dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="342dc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="342dc-110">Permission type</span></span>|<span data-ttu-id="342dc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="342dc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="342dc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="342dc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="342dc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="342dc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="342dc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="342dc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="342dc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="342dc-115">Not supported.</span></span>|
|<span data-ttu-id="342dc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="342dc-116">Application</span></span>|<span data-ttu-id="342dc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="342dc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="342dc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="342dc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="342dc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="342dc-119">Request headers</span></span>
|<span data-ttu-id="342dc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="342dc-120">Header</span></span>|<span data-ttu-id="342dc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="342dc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="342dc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="342dc-122">Authorization</span></span>|<span data-ttu-id="342dc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="342dc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="342dc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="342dc-124">Accept</span></span>|<span data-ttu-id="342dc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="342dc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="342dc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="342dc-126">Request body</span></span>
<span data-ttu-id="342dc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="342dc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="342dc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="342dc-128">Response</span></span>
<span data-ttu-id="342dc-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="342dc-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="342dc-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="342dc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="342dc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="342dc-131">Request</span></span>
<span data-ttu-id="342dc-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="342dc-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="342dc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="342dc-133">Response</span></span>
<span data-ttu-id="342dc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="342dc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









