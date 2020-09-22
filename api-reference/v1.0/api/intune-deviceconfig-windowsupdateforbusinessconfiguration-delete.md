---
title: Excluir windowsUpdateForBusinessConfiguration
description: Exclui windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a76a24cf6d97e035a3c92cc2e37edebe36aa396e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063216"
---
# <a name="delete-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="52c62-103">Excluir windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="52c62-103">Delete windowsUpdateForBusinessConfiguration</span></span>

<span data-ttu-id="52c62-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52c62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52c62-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52c62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52c62-106">Exclui [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="52c62-106">Deletes a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52c62-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52c62-107">Prerequisites</span></span>
<span data-ttu-id="52c62-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52c62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52c62-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52c62-110">Permission type</span></span>|<span data-ttu-id="52c62-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="52c62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52c62-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52c62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="52c62-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52c62-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="52c62-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52c62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52c62-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52c62-115">Not supported.</span></span>|
|<span data-ttu-id="52c62-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52c62-116">Application</span></span>|<span data-ttu-id="52c62-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52c62-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52c62-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52c62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="52c62-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52c62-119">Request headers</span></span>
|<span data-ttu-id="52c62-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52c62-120">Header</span></span>|<span data-ttu-id="52c62-121">Valor</span><span class="sxs-lookup"><span data-stu-id="52c62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52c62-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="52c62-122">Authorization</span></span>|<span data-ttu-id="52c62-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52c62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52c62-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="52c62-124">Accept</span></span>|<span data-ttu-id="52c62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="52c62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52c62-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52c62-126">Request body</span></span>
<span data-ttu-id="52c62-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52c62-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52c62-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="52c62-128">Response</span></span>
<span data-ttu-id="52c62-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="52c62-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="52c62-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52c62-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="52c62-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52c62-131">Request</span></span>
<span data-ttu-id="52c62-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52c62-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="52c62-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="52c62-133">Response</span></span>
<span data-ttu-id="52c62-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52c62-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









