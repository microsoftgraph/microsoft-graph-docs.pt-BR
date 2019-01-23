---
title: Criar managedEBookAssignment
description: Criar um novo objeto managedEBookAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f1f00c4db40b157359fd04171df6799d56949caa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409556"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="571fd-103">Criar managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="571fd-103">Create managedEBookAssignment</span></span>

> <span data-ttu-id="571fd-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="571fd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="571fd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="571fd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="571fd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="571fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="571fd-107">Criar um novo objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="571fd-107">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="571fd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="571fd-108">Prerequisites</span></span>
<span data-ttu-id="571fd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="571fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="571fd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="571fd-111">Permission type</span></span>|<span data-ttu-id="571fd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="571fd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="571fd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="571fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="571fd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="571fd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="571fd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="571fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="571fd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="571fd-116">Not supported.</span></span>|
|<span data-ttu-id="571fd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="571fd-117">Application</span></span>|<span data-ttu-id="571fd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="571fd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="571fd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="571fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="571fd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="571fd-120">Request headers</span></span>
|<span data-ttu-id="571fd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="571fd-121">Header</span></span>|<span data-ttu-id="571fd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="571fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="571fd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="571fd-123">Authorization</span></span>|<span data-ttu-id="571fd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="571fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="571fd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="571fd-125">Accept</span></span>|<span data-ttu-id="571fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="571fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="571fd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="571fd-127">Request body</span></span>
<span data-ttu-id="571fd-128">No corpo da solicitação, forneça uma representação JSON do objeto managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="571fd-128">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="571fd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="571fd-129">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="571fd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="571fd-130">Property</span></span>|<span data-ttu-id="571fd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="571fd-131">Type</span></span>|<span data-ttu-id="571fd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="571fd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="571fd-133">id</span><span class="sxs-lookup"><span data-stu-id="571fd-133">id</span></span>|<span data-ttu-id="571fd-134">String</span><span class="sxs-lookup"><span data-stu-id="571fd-134">String</span></span>|<span data-ttu-id="571fd-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="571fd-135">Key of the entity.</span></span>|
|<span data-ttu-id="571fd-136">destino</span><span class="sxs-lookup"><span data-stu-id="571fd-136">target</span></span>|[<span data-ttu-id="571fd-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="571fd-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="571fd-138">O destino da atribuição do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="571fd-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="571fd-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="571fd-139">installIntent</span></span>|[<span data-ttu-id="571fd-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="571fd-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="571fd-141">A tentativa de instalação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="571fd-141">The install intent for eBook.</span></span> <span data-ttu-id="571fd-142">Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="571fd-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="571fd-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="571fd-143">Response</span></span>
<span data-ttu-id="571fd-144">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="571fd-144">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="571fd-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="571fd-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="571fd-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="571fd-146">Request</span></span>
<span data-ttu-id="571fd-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="571fd-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 194

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="571fd-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="571fd-148">Response</span></span>
<span data-ttu-id="571fd-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="571fd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```




