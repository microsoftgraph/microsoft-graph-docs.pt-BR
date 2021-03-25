---
title: Atualizar roleManagement
description: Atualize as propriedades de um objeto roleManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 549d3ab5bc3e4d248ba81bf5c0059a6fcd0d5e90
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156671"
---
# <a name="update-rolemanagement"></a><span data-ttu-id="90086-103">Atualizar roleManagement</span><span class="sxs-lookup"><span data-stu-id="90086-103">Update roleManagement</span></span>

<span data-ttu-id="90086-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90086-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90086-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="90086-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90086-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90086-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90086-107">Atualize as propriedades de um [objeto roleManagement.](../resources/intune-rbac-rolemanagement.md)</span><span class="sxs-lookup"><span data-stu-id="90086-107">Update the properties of a [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90086-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90086-108">Prerequisites</span></span>
<span data-ttu-id="90086-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90086-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90086-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90086-111">Permission type</span></span>|<span data-ttu-id="90086-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90086-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90086-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90086-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90086-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90086-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="90086-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90086-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90086-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90086-116">Not supported.</span></span>|
|<span data-ttu-id="90086-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90086-117">Application</span></span>|<span data-ttu-id="90086-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90086-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90086-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90086-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement
```

## <a name="request-headers"></a><span data-ttu-id="90086-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90086-120">Request headers</span></span>
|<span data-ttu-id="90086-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90086-121">Header</span></span>|<span data-ttu-id="90086-122">Valor</span><span class="sxs-lookup"><span data-stu-id="90086-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90086-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="90086-123">Authorization</span></span>|<span data-ttu-id="90086-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90086-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90086-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90086-125">Accept</span></span>|<span data-ttu-id="90086-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90086-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90086-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90086-127">Request body</span></span>
<span data-ttu-id="90086-128">No corpo da solicitação, fornece uma representação JSON para o [objeto roleManagement.](../resources/intune-rbac-rolemanagement.md)</span><span class="sxs-lookup"><span data-stu-id="90086-128">In the request body, supply a JSON representation for the [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>

<span data-ttu-id="90086-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [a funçãoManagement](../resources/intune-rbac-rolemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="90086-129">The following table shows the properties that are required when you create the [roleManagement](../resources/intune-rbac-rolemanagement.md).</span></span>

|<span data-ttu-id="90086-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90086-130">Property</span></span>|<span data-ttu-id="90086-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="90086-131">Type</span></span>|<span data-ttu-id="90086-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="90086-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90086-133">id</span><span class="sxs-lookup"><span data-stu-id="90086-133">id</span></span>|<span data-ttu-id="90086-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90086-134">String</span></span>|<span data-ttu-id="90086-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="90086-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="90086-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="90086-136">Response</span></span>
<span data-ttu-id="90086-137">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [roleManagement](../resources/intune-rbac-rolemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90086-137">If successful, this method returns a `200 OK` response code and an updated [roleManagement](../resources/intune-rbac-rolemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90086-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90086-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="90086-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90086-139">Request</span></span>
<span data-ttu-id="90086-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90086-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/roleManagement
Content-type: application/json
Content-length: 56

{
  "@odata.type": "#microsoft.graph.roleManagement"
}
```

### <a name="response"></a><span data-ttu-id="90086-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="90086-141">Response</span></span>
<span data-ttu-id="90086-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90086-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 105

{
  "@odata.type": "#microsoft.graph.roleManagement",
  "id": "6fb74c1e-4c1e-6fb7-1e4c-b76f1e4cb76f"
}
```




