---
title: Excluir mobileAppAssignment
description: Exclui mobileAppAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f62f2fd63c503aa9de90292985bc034079a5422b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355138"
---
# <a name="delete-mobileappassignment"></a><span data-ttu-id="ecaec-103">Excluir mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="ecaec-103">Delete mobileAppAssignment</span></span>

> <span data-ttu-id="ecaec-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ecaec-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecaec-105">Exclui [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ecaec-105">Deletes a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecaec-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ecaec-106">Prerequisites</span></span>
<span data-ttu-id="ecaec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecaec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecaec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ecaec-109">Permission type</span></span>|<span data-ttu-id="ecaec-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ecaec-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecaec-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ecaec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ecaec-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecaec-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ecaec-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ecaec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecaec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecaec-114">Not supported.</span></span>|
|<span data-ttu-id="ecaec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ecaec-115">Application</span></span>|<span data-ttu-id="ecaec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecaec-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecaec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecaec-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ecaec-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecaec-118">Request headers</span></span>
|<span data-ttu-id="ecaec-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ecaec-119">Header</span></span>|<span data-ttu-id="ecaec-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ecaec-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecaec-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecaec-121">Authorization</span></span>|<span data-ttu-id="ecaec-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecaec-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecaec-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ecaec-123">Accept</span></span>|<span data-ttu-id="ecaec-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ecaec-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecaec-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecaec-125">Request body</span></span>
<span data-ttu-id="ecaec-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ecaec-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecaec-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecaec-127">Response</span></span>
<span data-ttu-id="ecaec-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ecaec-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ecaec-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ecaec-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecaec-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ecaec-130">Request</span></span>
<span data-ttu-id="ecaec-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecaec-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="ecaec-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecaec-132">Response</span></span>
<span data-ttu-id="ecaec-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ecaec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




