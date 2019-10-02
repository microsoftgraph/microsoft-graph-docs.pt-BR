---
title: atribuir ação
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 16ac39e8eb0092b7e8613aaddf18ef6913a874e4
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354718"
---
# <a name="assign-action"></a><span data-ttu-id="13452-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="13452-103">assign action</span></span>

> <span data-ttu-id="13452-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13452-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13452-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="13452-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13452-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13452-106">Prerequisites</span></span>
<span data-ttu-id="13452-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13452-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13452-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13452-109">Permission type</span></span>|<span data-ttu-id="13452-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13452-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13452-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13452-111">Delegated (work or school account)</span></span>|<span data-ttu-id="13452-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13452-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="13452-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13452-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13452-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13452-114">Not supported.</span></span>|
|<span data-ttu-id="13452-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13452-115">Application</span></span>|<span data-ttu-id="13452-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13452-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13452-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13452-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="13452-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13452-118">Request headers</span></span>
|<span data-ttu-id="13452-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13452-119">Header</span></span>|<span data-ttu-id="13452-120">Valor</span><span class="sxs-lookup"><span data-stu-id="13452-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13452-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="13452-121">Authorization</span></span>|<span data-ttu-id="13452-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13452-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13452-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13452-123">Accept</span></span>|<span data-ttu-id="13452-124">application/json</span><span class="sxs-lookup"><span data-stu-id="13452-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13452-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13452-125">Request body</span></span>
<span data-ttu-id="13452-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="13452-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="13452-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="13452-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="13452-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13452-128">Property</span></span>|<span data-ttu-id="13452-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="13452-129">Type</span></span>|<span data-ttu-id="13452-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="13452-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13452-131">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="13452-131">managedEBookAssignments</span></span>|<span data-ttu-id="13452-132">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="13452-132">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="13452-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="13452-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="13452-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="13452-134">Response</span></span>
<span data-ttu-id="13452-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="13452-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="13452-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13452-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="13452-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13452-137">Request</span></span>
<span data-ttu-id="13452-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13452-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assign

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

### <a name="response"></a><span data-ttu-id="13452-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="13452-139">Response</span></span>
<span data-ttu-id="13452-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13452-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




