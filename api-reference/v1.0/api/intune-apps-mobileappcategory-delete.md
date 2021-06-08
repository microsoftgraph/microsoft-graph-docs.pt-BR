---
title: Excluir mobileAppCategory
description: Exclui mobileAppCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e1658551fef9731bd97f3f90c7fd791222180680
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759718"
---
# <a name="delete-mobileappcategory"></a><span data-ttu-id="baebf-103">Excluir mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="baebf-103">Delete mobileAppCategory</span></span>

<span data-ttu-id="baebf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="baebf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="baebf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="baebf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="baebf-106">Exclui [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="baebf-106">Deletes a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="baebf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="baebf-107">Prerequisites</span></span>
<span data-ttu-id="baebf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baebf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baebf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="baebf-110">Permission type</span></span>|<span data-ttu-id="baebf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="baebf-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="baebf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="baebf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="baebf-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baebf-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="baebf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="baebf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="baebf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="baebf-115">Not supported.</span></span>|
|<span data-ttu-id="baebf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="baebf-116">Application</span></span>|<span data-ttu-id="baebf-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baebf-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="baebf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="baebf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="baebf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="baebf-119">Request headers</span></span>
|<span data-ttu-id="baebf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="baebf-120">Header</span></span>|<span data-ttu-id="baebf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="baebf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="baebf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="baebf-122">Authorization</span></span>|<span data-ttu-id="baebf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="baebf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="baebf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="baebf-124">Accept</span></span>|<span data-ttu-id="baebf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="baebf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="baebf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="baebf-126">Request body</span></span>
<span data-ttu-id="baebf-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="baebf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="baebf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="baebf-128">Response</span></span>
<span data-ttu-id="baebf-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="baebf-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="baebf-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="baebf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="baebf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="baebf-131">Request</span></span>
<span data-ttu-id="baebf-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="baebf-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
```

### <a name="response"></a><span data-ttu-id="baebf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="baebf-133">Response</span></span>
<span data-ttu-id="baebf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="baebf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




