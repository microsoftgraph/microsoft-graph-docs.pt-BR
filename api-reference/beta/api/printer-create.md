---
title: 'impressora: criar'
description: Cria (registra) uma impressora com o serviço de impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8080185c913a99702fba9510845ac284bf186afc
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314376"
---
# <a name="printer-create"></a><span data-ttu-id="0df87-103">impressora: criar</span><span class="sxs-lookup"><span data-stu-id="0df87-103">printer: create</span></span>

<span data-ttu-id="0df87-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0df87-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0df87-105">Criar (registrar) uma impressora com o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="0df87-105">Create (register) a printer with the Universal Print service.</span></span> <span data-ttu-id="0df87-106">Esta é uma operação de execução demorada e, como tal, retorna um [printerCreateOperation](../resources/printercreateoperation.md) que pode ser usado para rastrear e verificar o registro da impressora.</span><span class="sxs-lookup"><span data-stu-id="0df87-106">This is a long-running operation and as such, it returns a [printerCreateOperation](../resources/printercreateoperation.md) that can be used to track and verify the registration of the printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="0df87-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0df87-107">Permissions</span></span>
<span data-ttu-id="0df87-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0df87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0df87-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="0df87-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="0df87-111">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="0df87-111">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="0df87-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0df87-112">Permission type</span></span> | <span data-ttu-id="0df87-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0df87-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0df87-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0df87-114">Delegated (work or school account)</span></span>| <span data-ttu-id="0df87-115">Printer. Create, Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="0df87-115">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="0df87-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0df87-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0df87-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0df87-117">Not Supported.</span></span>|
|<span data-ttu-id="0df87-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0df87-118">Application</span></span>| <span data-ttu-id="0df87-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0df87-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0df87-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0df87-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/create
```
## <a name="request-headers"></a><span data-ttu-id="0df87-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0df87-121">Request headers</span></span>
| <span data-ttu-id="0df87-122">Nome</span><span class="sxs-lookup"><span data-stu-id="0df87-122">Name</span></span>       | <span data-ttu-id="0df87-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0df87-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0df87-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0df87-124">Authorization</span></span> | <span data-ttu-id="0df87-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0df87-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0df87-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="0df87-127">Content-type</span></span>  | <span data-ttu-id="0df87-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0df87-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0df87-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0df87-130">Request body</span></span>
<span data-ttu-id="0df87-131">No corpo da solicitação, forneça um objeto JSON com as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="0df87-131">In the request body, provide a JSON object with the following properties.</span></span>

| <span data-ttu-id="0df87-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0df87-132">Parameter</span></span>      | <span data-ttu-id="0df87-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="0df87-133">Type</span></span>    |<span data-ttu-id="0df87-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="0df87-134">Description</span></span>| <span data-ttu-id="0df87-135">Obrigatório?</span><span class="sxs-lookup"><span data-stu-id="0df87-135">Required?</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="0df87-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0df87-136">displayName</span></span>|<span data-ttu-id="0df87-137">String</span><span class="sxs-lookup"><span data-stu-id="0df87-137">String</span></span>|<span data-ttu-id="0df87-138">O nome de exibição a ser atribuído à impressora.</span><span class="sxs-lookup"><span data-stu-id="0df87-138">The display name to assign to the printer.</span></span>|<span data-ttu-id="0df87-139">Sim</span><span class="sxs-lookup"><span data-stu-id="0df87-139">Yes</span></span>|
|<span data-ttu-id="0df87-140">fabricante</span><span class="sxs-lookup"><span data-stu-id="0df87-140">manufacturer</span></span>|<span data-ttu-id="0df87-141">String</span><span class="sxs-lookup"><span data-stu-id="0df87-141">String</span></span>|<span data-ttu-id="0df87-142">O fabricante da impressora.</span><span class="sxs-lookup"><span data-stu-id="0df87-142">The manufacturer of the printer.</span></span>|<span data-ttu-id="0df87-143">Sim</span><span class="sxs-lookup"><span data-stu-id="0df87-143">Yes</span></span>|
|<span data-ttu-id="0df87-144">modelo</span><span class="sxs-lookup"><span data-stu-id="0df87-144">model</span></span>|<span data-ttu-id="0df87-145">String</span><span class="sxs-lookup"><span data-stu-id="0df87-145">String</span></span>|<span data-ttu-id="0df87-146">O modelo da impressora.</span><span class="sxs-lookup"><span data-stu-id="0df87-146">The model of the printer.</span></span>|<span data-ttu-id="0df87-147">Sim</span><span class="sxs-lookup"><span data-stu-id="0df87-147">Yes</span></span>|
|<span data-ttu-id="0df87-148">physicalDeviceId</span><span class="sxs-lookup"><span data-stu-id="0df87-148">physicalDeviceId</span></span>|<span data-ttu-id="0df87-149">String</span><span class="sxs-lookup"><span data-stu-id="0df87-149">String</span></span>|<span data-ttu-id="0df87-150">O UUID do dispositivo físico da impressora.</span><span class="sxs-lookup"><span data-stu-id="0df87-150">The physical device UUID of the printer.</span></span> <span data-ttu-id="0df87-151">Obrigatório se a `hasPhysicalDevice` propriedade for true.</span><span class="sxs-lookup"><span data-stu-id="0df87-151">Required if the `hasPhysicalDevice` property is true.</span></span>|<span data-ttu-id="0df87-152">Não</span><span class="sxs-lookup"><span data-stu-id="0df87-152">No</span></span>|
|<span data-ttu-id="0df87-153">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="0df87-153">hasPhysicalDevice</span></span>|<span data-ttu-id="0df87-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="0df87-154">Boolean</span></span>|<span data-ttu-id="0df87-155">True se a impressora tem dispositivo de saída físico; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="0df87-155">True if the printer has physical output device, false otherwise.</span></span> <span data-ttu-id="0df87-156">Se for omitido, o valor padrão será true.</span><span class="sxs-lookup"><span data-stu-id="0df87-156">If omitted, the default value is true.</span></span>|<span data-ttu-id="0df87-157">Não</span><span class="sxs-lookup"><span data-stu-id="0df87-157">No</span></span>|
|<span data-ttu-id="0df87-158">certificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="0df87-158">certificateSigningRequest</span></span>|[<span data-ttu-id="0df87-159">printCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="0df87-159">printCertificateSigningRequest</span></span>](../resources/printcertificatesigningrequest.md)|<span data-ttu-id="0df87-160">A solicitação de assinatura de certificado (CSR) do X. 509 para o certificado criado e usado pela impressora para identificar-se.</span><span class="sxs-lookup"><span data-stu-id="0df87-160">The X.509 Certificate Signing Request (CSR) for the certificate created and used by the printer to identify itself.</span></span>|<span data-ttu-id="0df87-161">Sim</span><span class="sxs-lookup"><span data-stu-id="0df87-161">Yes</span></span>|
|<span data-ttu-id="0df87-162">connectorid</span><span class="sxs-lookup"><span data-stu-id="0df87-162">connectorId</span></span>|<span data-ttu-id="0df87-163">String</span><span class="sxs-lookup"><span data-stu-id="0df87-163">String</span></span>|<span data-ttu-id="0df87-164">ID do conector que atua como proxy para a impressora.</span><span class="sxs-lookup"><span data-stu-id="0df87-164">Id of Connector acting as proxy to the printer.</span></span>|<span data-ttu-id="0df87-165">Não</span><span class="sxs-lookup"><span data-stu-id="0df87-165">No</span></span>|

## <a name="response"></a><span data-ttu-id="0df87-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="0df87-166">Response</span></span>
<span data-ttu-id="0df87-167">Se tiver êxito, este método retornará um `202 Accepted` código de resposta e um link para o [printerCreateOperation](../resources/printercreateoperation.md) associado no `Operation-Location` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="0df87-167">If successful, this method returns a `202 Accepted` response code and a link to the associated [printerCreateOperation](../resources/printercreateoperation.md) in the `Operation-Location` header.</span></span>

<span data-ttu-id="0df87-168">Fazer uma solicitação GET para a URL vinculada pode ser usado para obter o status de um registro de impressora em andamento.</span><span class="sxs-lookup"><span data-stu-id="0df87-168">Making a GET request to the linked URL can be used to get the status of an ongoing printer registration.</span></span> <span data-ttu-id="0df87-169">Após o registro da impressora ter sido concluído com êxito, uma solicitação GET para a URL vinculada conterá o objeto Printer criado e o certificado registrado.</span><span class="sxs-lookup"><span data-stu-id="0df87-169">Once printer registration has completed successfully, a GET request to the linked URL will contain the created printer object and registered certificate.</span></span>

## <a name="example"></a><span data-ttu-id="0df87-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0df87-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="0df87-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0df87-171">Request</span></span>
<span data-ttu-id="0df87-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0df87-172">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0df87-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="0df87-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printer"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/create
Content-type: application/json
Content-length: 319

{
  "displayName": "Test Printer",
  "manufacturer": "Test Printer Manufacturer",
  "model": "Test Printer Model",
  "physicalDeviceId": null,
  "hasPhysicalDevice": false,
  "certificateSigningRequest": { 
    "content": "{content}",
    "transportKey": "{sampleTransportKey}"
  },
  "connectorId": null
}
```
# <a name="javascript"></a>[<span data-ttu-id="0df87-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0df87-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="0df87-175">C#</span><span class="sxs-lookup"><span data-stu-id="0df87-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0df87-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0df87-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0df87-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="0df87-177">Response</span></span>
<span data-ttu-id="0df87-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0df87-178">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Operation-Location: https://graph.microsoft.com/beta/print/operations/f221760a-52e8-4c11-b8c5-5dfaef3a49db
Retry-After: 5
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printers: create",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
