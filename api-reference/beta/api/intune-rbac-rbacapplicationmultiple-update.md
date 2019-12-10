---
title: Atualizar rbacApplicationMultiple
description: Atualiza as propriedades de um objeto rbacApplicationMultiple.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5d0d835f328bf68efe09aa55f853a0e713b1e41c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940781"
---
# <a name="update-rbacapplicationmultiple"></a><span data-ttu-id="81641-103">Atualizar rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="81641-103">Update rbacApplicationMultiple</span></span>

> <span data-ttu-id="81641-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81641-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81641-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81641-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81641-106">Atualiza as propriedades de um objeto [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="81641-106">Update the properties of a [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81641-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81641-107">Prerequisites</span></span>
<span data-ttu-id="81641-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81641-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81641-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81641-110">Permission type</span></span>|<span data-ttu-id="81641-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81641-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81641-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81641-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81641-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81641-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="81641-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81641-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81641-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81641-115">Not supported.</span></span>|
|<span data-ttu-id="81641-116">Application</span><span class="sxs-lookup"><span data-stu-id="81641-116">Application</span></span>|<span data-ttu-id="81641-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81641-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81641-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81641-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement/deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="81641-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81641-119">Request headers</span></span>
|<span data-ttu-id="81641-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81641-120">Header</span></span>|<span data-ttu-id="81641-121">Valor</span><span class="sxs-lookup"><span data-stu-id="81641-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81641-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="81641-122">Authorization</span></span>|<span data-ttu-id="81641-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81641-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81641-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81641-124">Accept</span></span>|<span data-ttu-id="81641-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81641-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81641-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81641-126">Request body</span></span>
<span data-ttu-id="81641-127">No corpo da solicitação, forneça uma representação JSON do objeto [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="81641-127">In the request body, supply a JSON representation for the [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object.</span></span>

<span data-ttu-id="81641-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md).</span><span class="sxs-lookup"><span data-stu-id="81641-128">The following table shows the properties that are required when you create the [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md).</span></span>

|<span data-ttu-id="81641-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81641-129">Property</span></span>|<span data-ttu-id="81641-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="81641-130">Type</span></span>|<span data-ttu-id="81641-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="81641-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81641-132">id</span><span class="sxs-lookup"><span data-stu-id="81641-132">id</span></span>|<span data-ttu-id="81641-133">String</span><span class="sxs-lookup"><span data-stu-id="81641-133">String</span></span>|<span data-ttu-id="81641-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="81641-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="81641-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="81641-135">Response</span></span>
<span data-ttu-id="81641-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81641-136">If successful, this method returns a `200 OK` response code and an updated [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81641-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81641-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="81641-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81641-138">Request</span></span>
<span data-ttu-id="81641-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81641-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/deviceManagement
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.rbacApplicationMultiple"
}
```

### <a name="response"></a><span data-ttu-id="81641-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="81641-140">Response</span></span>
<span data-ttu-id="81641-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81641-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.rbacApplicationMultiple",
  "id": "ee4797e5-97e5-ee47-e597-47eee59747ee"
}
```





