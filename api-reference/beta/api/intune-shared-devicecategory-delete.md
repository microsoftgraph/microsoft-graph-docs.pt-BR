---
title: Excluir deviceCategory
description: Exclui deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b01adf8559c204a8d86beb344bde3dd972e6d468
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980418"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="241b9-103">Excluir deviceCategory</span><span class="sxs-lookup"><span data-stu-id="241b9-103">Delete deviceCategory</span></span>

<span data-ttu-id="241b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="241b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="241b9-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="241b9-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="241b9-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="241b9-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="241b9-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="241b9-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="241b9-108">Exclui [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="241b9-108">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="241b9-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="241b9-109">Prerequisites</span></span>
<span data-ttu-id="241b9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="241b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="241b9-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="241b9-112">Permission type</span></span>|<span data-ttu-id="241b9-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="241b9-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="241b9-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="241b9-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="241b9-115">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="241b9-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="241b9-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="241b9-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="241b9-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="241b9-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="241b9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="241b9-118">Not supported.</span></span>|
|<span data-ttu-id="241b9-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="241b9-119">Application</span></span>||
| <span data-ttu-id="241b9-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="241b9-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="241b9-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="241b9-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="241b9-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="241b9-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="241b9-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="241b9-123">Request headers</span></span>
|<span data-ttu-id="241b9-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="241b9-124">Header</span></span>|<span data-ttu-id="241b9-125">Valor</span><span class="sxs-lookup"><span data-stu-id="241b9-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="241b9-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="241b9-126">Authorization</span></span>|<span data-ttu-id="241b9-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="241b9-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="241b9-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="241b9-128">Accept</span></span>|<span data-ttu-id="241b9-129">application/json</span><span class="sxs-lookup"><span data-stu-id="241b9-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="241b9-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="241b9-130">Request body</span></span>
<span data-ttu-id="241b9-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="241b9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="241b9-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="241b9-132">Response</span></span>
<span data-ttu-id="241b9-133">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="241b9-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="241b9-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="241b9-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="241b9-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="241b9-135">Request</span></span>

<span data-ttu-id="241b9-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="241b9-136">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="241b9-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="241b9-137">Response</span></span>

<span data-ttu-id="241b9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="241b9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```












