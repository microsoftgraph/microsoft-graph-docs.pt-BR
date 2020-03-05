---
title: Excluir managedEBookAssignment
description: Exclui managedEBookAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 49173d21b29b83ad2aa120f281b0725f07b51894
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450311"
---
# <a name="delete-managedebookassignment"></a><span data-ttu-id="02e83-103">Excluir managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="02e83-103">Delete managedEBookAssignment</span></span>

<span data-ttu-id="02e83-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="02e83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02e83-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02e83-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02e83-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02e83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02e83-107">Exclui [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="02e83-107">Deletes a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02e83-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02e83-108">Prerequisites</span></span>
<span data-ttu-id="02e83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02e83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02e83-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02e83-111">Permission type</span></span>|<span data-ttu-id="02e83-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02e83-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02e83-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02e83-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02e83-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02e83-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="02e83-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02e83-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02e83-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02e83-116">Not supported.</span></span>|
|<span data-ttu-id="02e83-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02e83-117">Application</span></span>|<span data-ttu-id="02e83-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02e83-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02e83-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02e83-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="02e83-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02e83-120">Request headers</span></span>
|<span data-ttu-id="02e83-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02e83-121">Header</span></span>|<span data-ttu-id="02e83-122">Valor</span><span class="sxs-lookup"><span data-stu-id="02e83-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02e83-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="02e83-123">Authorization</span></span>|<span data-ttu-id="02e83-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02e83-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02e83-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02e83-125">Accept</span></span>|<span data-ttu-id="02e83-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02e83-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02e83-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02e83-127">Request body</span></span>
<span data-ttu-id="02e83-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02e83-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02e83-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="02e83-129">Response</span></span>
<span data-ttu-id="02e83-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="02e83-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="02e83-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02e83-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="02e83-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02e83-132">Request</span></span>
<span data-ttu-id="02e83-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02e83-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="02e83-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="02e83-134">Response</span></span>
<span data-ttu-id="02e83-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02e83-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





