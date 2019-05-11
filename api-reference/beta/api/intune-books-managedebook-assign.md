---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a180c1f6670c51f277e672a5480aa129312a1e36
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934240"
---
# <a name="assign-action"></a><span data-ttu-id="1255a-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="1255a-103">assign action</span></span>

> <span data-ttu-id="1255a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1255a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1255a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1255a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1255a-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1255a-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1255a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1255a-107">Prerequisites</span></span>
<span data-ttu-id="1255a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1255a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1255a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1255a-110">Permission type</span></span>|<span data-ttu-id="1255a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1255a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1255a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1255a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1255a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1255a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1255a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1255a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1255a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1255a-115">Not supported.</span></span>|
|<span data-ttu-id="1255a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1255a-116">Application</span></span>|<span data-ttu-id="1255a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1255a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1255a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1255a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="1255a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1255a-119">Request headers</span></span>
|<span data-ttu-id="1255a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1255a-120">Header</span></span>|<span data-ttu-id="1255a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1255a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1255a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1255a-122">Authorization</span></span>|<span data-ttu-id="1255a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1255a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1255a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1255a-124">Accept</span></span>|<span data-ttu-id="1255a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1255a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1255a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1255a-126">Request body</span></span>
<span data-ttu-id="1255a-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="1255a-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1255a-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="1255a-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1255a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1255a-129">Property</span></span>|<span data-ttu-id="1255a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1255a-130">Type</span></span>|<span data-ttu-id="1255a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1255a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1255a-132">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="1255a-132">managedEBookAssignments</span></span>|<span data-ttu-id="1255a-133">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1255a-133">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="1255a-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1255a-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1255a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1255a-135">Response</span></span>
<span data-ttu-id="1255a-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1255a-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1255a-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1255a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="1255a-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1255a-138">Request</span></span>
<span data-ttu-id="1255a-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1255a-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1255a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1255a-140">Response</span></span>
<span data-ttu-id="1255a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1255a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




