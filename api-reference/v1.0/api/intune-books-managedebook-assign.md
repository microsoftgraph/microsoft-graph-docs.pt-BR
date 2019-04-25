---
title: atribuir ação
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94c50cf4e3f880f61f1e392d9166c6dfe7a6f5ac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524904"
---
# <a name="assign-action"></a><span data-ttu-id="83000-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="83000-103">assign action</span></span>

> <span data-ttu-id="83000-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83000-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83000-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83000-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83000-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="83000-106">Prerequisites</span></span>
<span data-ttu-id="83000-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83000-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83000-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83000-109">Permission type</span></span>|<span data-ttu-id="83000-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="83000-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83000-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83000-111">Delegated (work or school account)</span></span>|<span data-ttu-id="83000-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83000-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="83000-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83000-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83000-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83000-114">Not supported.</span></span>|
|<span data-ttu-id="83000-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83000-115">Application</span></span>|<span data-ttu-id="83000-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83000-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83000-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83000-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="83000-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83000-118">Request headers</span></span>
|<span data-ttu-id="83000-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83000-119">Header</span></span>|<span data-ttu-id="83000-120">Valor</span><span class="sxs-lookup"><span data-stu-id="83000-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83000-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="83000-121">Authorization</span></span>|<span data-ttu-id="83000-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83000-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83000-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="83000-123">Accept</span></span>|<span data-ttu-id="83000-124">application/json</span><span class="sxs-lookup"><span data-stu-id="83000-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83000-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83000-125">Request body</span></span>
<span data-ttu-id="83000-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="83000-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="83000-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="83000-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="83000-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83000-128">Property</span></span>|<span data-ttu-id="83000-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="83000-129">Type</span></span>|<span data-ttu-id="83000-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="83000-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83000-131">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="83000-131">managedEBookAssignments</span></span>|<span data-ttu-id="83000-132">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="83000-132">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="83000-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="83000-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="83000-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="83000-134">Response</span></span>
<span data-ttu-id="83000-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="83000-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="83000-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83000-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="83000-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83000-137">Request</span></span>
<span data-ttu-id="83000-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83000-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="83000-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="83000-139">Response</span></span>
<span data-ttu-id="83000-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83000-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



