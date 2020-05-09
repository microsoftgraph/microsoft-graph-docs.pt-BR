---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 675b146e14516d897672e27cd38ea111cc150b49
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44175102"
---
# <a name="assign-action"></a><span data-ttu-id="2b780-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="2b780-103">assign action</span></span>

<span data-ttu-id="2b780-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b780-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b780-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2b780-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b780-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b780-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b780-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2b780-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b780-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2b780-108">Prerequisites</span></span>
<span data-ttu-id="2b780-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b780-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b780-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b780-111">Permission type</span></span>|<span data-ttu-id="2b780-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2b780-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b780-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b780-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b780-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b780-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2b780-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b780-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b780-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b780-116">Not supported.</span></span>|
|<span data-ttu-id="2b780-117">Application</span><span class="sxs-lookup"><span data-stu-id="2b780-117">Application</span></span>|<span data-ttu-id="2b780-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b780-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b780-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b780-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="2b780-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b780-120">Request headers</span></span>
|<span data-ttu-id="2b780-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2b780-121">Header</span></span>|<span data-ttu-id="2b780-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2b780-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b780-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b780-123">Authorization</span></span>|<span data-ttu-id="2b780-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b780-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b780-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2b780-125">Accept</span></span>|<span data-ttu-id="2b780-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b780-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b780-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b780-127">Request body</span></span>
<span data-ttu-id="2b780-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="2b780-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2b780-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="2b780-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2b780-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b780-130">Property</span></span>|<span data-ttu-id="2b780-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b780-131">Type</span></span>|<span data-ttu-id="2b780-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b780-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b780-133">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="2b780-133">managedEBookAssignments</span></span>|<span data-ttu-id="2b780-134">Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2b780-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="2b780-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2b780-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2b780-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b780-136">Response</span></span>
<span data-ttu-id="2b780-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2b780-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2b780-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b780-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b780-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b780-139">Request</span></span>
<span data-ttu-id="2b780-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b780-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assign

Content-type: application/json
Content-length: 312

{
  "managedEBookAssignments": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="2b780-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b780-141">Response</span></span>
<span data-ttu-id="2b780-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b780-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



