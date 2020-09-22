---
title: Excluir windowsPhone81CustomConfiguration
description: Exclui windowsPhone81CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fa5b40592b4414c3386308fb4eee8365a0f041ba
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069803"
---
# <a name="delete-windowsphone81customconfiguration"></a><span data-ttu-id="02756-103">Excluir windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="02756-103">Delete windowsPhone81CustomConfiguration</span></span>

<span data-ttu-id="02756-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02756-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02756-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02756-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02756-106">Exclui [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02756-106">Deletes a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02756-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02756-107">Prerequisites</span></span>
<span data-ttu-id="02756-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02756-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02756-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02756-110">Permission type</span></span>|<span data-ttu-id="02756-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02756-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02756-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02756-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02756-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02756-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="02756-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02756-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02756-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02756-115">Not supported.</span></span>|
|<span data-ttu-id="02756-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02756-116">Application</span></span>|<span data-ttu-id="02756-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02756-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02756-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02756-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="02756-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02756-119">Request headers</span></span>
|<span data-ttu-id="02756-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02756-120">Header</span></span>|<span data-ttu-id="02756-121">Valor</span><span class="sxs-lookup"><span data-stu-id="02756-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02756-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="02756-122">Authorization</span></span>|<span data-ttu-id="02756-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02756-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02756-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02756-124">Accept</span></span>|<span data-ttu-id="02756-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02756-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02756-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02756-126">Request body</span></span>
<span data-ttu-id="02756-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02756-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02756-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="02756-128">Response</span></span>
<span data-ttu-id="02756-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="02756-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="02756-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02756-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="02756-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02756-131">Request</span></span>
<span data-ttu-id="02756-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02756-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="02756-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="02756-133">Response</span></span>
<span data-ttu-id="02756-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02756-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









