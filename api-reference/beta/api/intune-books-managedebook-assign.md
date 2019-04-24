---
title: atribuir ação
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6865ef77b442f8e22aa3d6fa50d37c87fc207c3a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32483240"
---
# <a name="assign-action"></a><span data-ttu-id="c5173-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="c5173-103">assign action</span></span>

> <span data-ttu-id="c5173-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c5173-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5173-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5173-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5173-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c5173-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5173-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c5173-107">Prerequisites</span></span>
<span data-ttu-id="c5173-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5173-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5173-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5173-110">Permission type</span></span>|<span data-ttu-id="c5173-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c5173-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5173-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5173-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5173-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5173-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c5173-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5173-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5173-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5173-115">Not supported.</span></span>|
|<span data-ttu-id="c5173-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5173-116">Application</span></span>|<span data-ttu-id="c5173-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5173-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5173-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5173-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="c5173-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5173-119">Request headers</span></span>
|<span data-ttu-id="c5173-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5173-120">Header</span></span>|<span data-ttu-id="c5173-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c5173-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5173-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5173-122">Authorization</span></span>|<span data-ttu-id="c5173-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5173-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5173-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c5173-124">Accept</span></span>|<span data-ttu-id="c5173-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5173-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5173-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5173-126">Request body</span></span>
<span data-ttu-id="c5173-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c5173-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c5173-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="c5173-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c5173-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5173-129">Property</span></span>|<span data-ttu-id="c5173-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5173-130">Type</span></span>|<span data-ttu-id="c5173-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5173-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5173-132">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="c5173-132">managedEBookAssignments</span></span>|<span data-ttu-id="c5173-133">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c5173-133">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="c5173-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c5173-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c5173-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5173-135">Response</span></span>
<span data-ttu-id="c5173-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c5173-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c5173-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5173-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5173-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5173-138">Request</span></span>
<span data-ttu-id="c5173-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5173-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assign

Content-type: application/json
Content-length: 318

{
  "managedEBookAssignments": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c5173-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5173-140">Response</span></span>
<span data-ttu-id="c5173-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5173-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





