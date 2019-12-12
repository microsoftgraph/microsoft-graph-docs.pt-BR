---
title: Atualizar roleManagement
description: Atualiza as propriedades de um objeto roleManagement.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b2451397f5bde92f949174edef67c311ff1d966c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955172"
---
# <a name="update-rolemanagement"></a><span data-ttu-id="eeec1-103">Atualizar roleManagement</span><span class="sxs-lookup"><span data-stu-id="eeec1-103">Update roleManagement</span></span>

> <span data-ttu-id="eeec1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eeec1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eeec1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eeec1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eeec1-106">Atualiza as propriedades de um objeto [roleManagement](../resources/intune-rbac-rolemanagement.md) .</span><span class="sxs-lookup"><span data-stu-id="eeec1-106">Update the properties of a [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eeec1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eeec1-107">Prerequisites</span></span>
<span data-ttu-id="eeec1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eeec1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeec1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eeec1-110">Permission type</span></span>|<span data-ttu-id="eeec1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eeec1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eeec1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eeec1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eeec1-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eeec1-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="eeec1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eeec1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eeec1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eeec1-115">Not supported.</span></span>|
|<span data-ttu-id="eeec1-116">Application</span><span class="sxs-lookup"><span data-stu-id="eeec1-116">Application</span></span>|<span data-ttu-id="eeec1-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eeec1-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eeec1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eeec1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement
```

## <a name="request-headers"></a><span data-ttu-id="eeec1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eeec1-119">Request headers</span></span>
|<span data-ttu-id="eeec1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eeec1-120">Header</span></span>|<span data-ttu-id="eeec1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eeec1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eeec1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eeec1-122">Authorization</span></span>|<span data-ttu-id="eeec1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eeec1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eeec1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eeec1-124">Accept</span></span>|<span data-ttu-id="eeec1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eeec1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eeec1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eeec1-126">Request body</span></span>
<span data-ttu-id="eeec1-127">No corpo da solicitação, forneça uma representação JSON do objeto [roleManagement](../resources/intune-rbac-rolemanagement.md) .</span><span class="sxs-lookup"><span data-stu-id="eeec1-127">In the request body, supply a JSON representation for the [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>

<span data-ttu-id="eeec1-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleManagement](../resources/intune-rbac-rolemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="eeec1-128">The following table shows the properties that are required when you create the [roleManagement](../resources/intune-rbac-rolemanagement.md).</span></span>

|<span data-ttu-id="eeec1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eeec1-129">Property</span></span>|<span data-ttu-id="eeec1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eeec1-130">Type</span></span>|<span data-ttu-id="eeec1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eeec1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eeec1-132">id</span><span class="sxs-lookup"><span data-stu-id="eeec1-132">id</span></span>|<span data-ttu-id="eeec1-133">String</span><span class="sxs-lookup"><span data-stu-id="eeec1-133">String</span></span>|<span data-ttu-id="eeec1-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="eeec1-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="eeec1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="eeec1-135">Response</span></span>
<span data-ttu-id="eeec1-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [roleManagement](../resources/intune-rbac-rolemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eeec1-136">If successful, this method returns a `200 OK` response code and an updated [roleManagement](../resources/intune-rbac-rolemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eeec1-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eeec1-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="eeec1-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eeec1-138">Request</span></span>
<span data-ttu-id="eeec1-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eeec1-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/roleManagement
Content-type: application/json
Content-length: 56

{
  "@odata.type": "#microsoft.graph.roleManagement"
}
```

### <a name="response"></a><span data-ttu-id="eeec1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="eeec1-140">Response</span></span>
<span data-ttu-id="eeec1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eeec1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 105

{
  "@odata.type": "#microsoft.graph.roleManagement",
  "id": "6fb74c1e-4c1e-6fb7-1e4c-b76f1e4cb76f"
}
```





