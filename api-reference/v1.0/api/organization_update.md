# <a name="update-organization"></a><span data-ttu-id="68e9a-101">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="68e9a-101">Update organization</span></span>

<span data-ttu-id="68e9a-102">Atualize as propriedades da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="68e9a-102">Update the properties of the currently authenticated organization.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68e9a-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="68e9a-103">Prerequisites</span></span>
<span data-ttu-id="68e9a-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="68e9a-104">One of the following **scopes** is required to execute this API:</span></span>
## <a name="http-request"></a><span data-ttu-id="68e9a-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68e9a-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /organization

```
## <a name="request-headers"></a><span data-ttu-id="68e9a-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68e9a-106">Request headers</span></span>
| <span data-ttu-id="68e9a-107">Nome</span><span class="sxs-lookup"><span data-stu-id="68e9a-107">Name</span></span>       | <span data-ttu-id="68e9a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="68e9a-108">Type</span></span> | <span data-ttu-id="68e9a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="68e9a-109">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="68e9a-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="68e9a-110">Authorization</span></span>  | <span data-ttu-id="68e9a-111">string</span><span class="sxs-lookup"><span data-stu-id="68e9a-111">string</span></span>  | <span data-ttu-id="68e9a-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68e9a-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68e9a-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68e9a-114">Request body</span></span>
<span data-ttu-id="68e9a-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="68e9a-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="68e9a-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68e9a-118">Property</span></span>     | <span data-ttu-id="68e9a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="68e9a-119">Type</span></span>   |<span data-ttu-id="68e9a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="68e9a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68e9a-121">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="68e9a-121">assignedPlans</span></span>|<span data-ttu-id="68e9a-122">AssignedPlan</span><span class="sxs-lookup"><span data-stu-id="68e9a-122">AssignedPlan</span></span>|<span data-ttu-id="68e9a-p103">A coleção de planos de serviço associados ao locatário.                            **Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="68e9a-p103">The collection of service plans associated with the tenant.                            **Notes**: not nullable.</span></span>            |
|<span data-ttu-id="68e9a-125">cidade</span><span class="sxs-lookup"><span data-stu-id="68e9a-125">city</span></span>|<span data-ttu-id="68e9a-126">String</span><span class="sxs-lookup"><span data-stu-id="68e9a-126">String</span></span>|            |
|<span data-ttu-id="68e9a-127">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="68e9a-127">companyLastDirSyncTime</span></span>|<span data-ttu-id="68e9a-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68e9a-128">DateTimeOffset</span></span>|<span data-ttu-id="68e9a-129">A hora e a data em que o locatário foi sincronizado pela última vez com o diretório local.</span><span class="sxs-lookup"><span data-stu-id="68e9a-129">The time and date at which the tenant was last synced with the on-premise directory.</span></span>|
|<span data-ttu-id="68e9a-130">país</span><span class="sxs-lookup"><span data-stu-id="68e9a-130">country</span></span>|<span data-ttu-id="68e9a-131">String</span><span class="sxs-lookup"><span data-stu-id="68e9a-131">String</span></span>|            |
|<span data-ttu-id="68e9a-132">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="68e9a-132">countryLetterCode</span></span>|<span data-ttu-id="68e9a-133">String</span><span class="sxs-lookup"><span data-stu-id="68e9a-133">String</span></span>|            |
|<span data-ttu-id="68e9a-134">deletionTimestamp</span><span class="sxs-lookup"><span data-stu-id="68e9a-134">deletionTimestamp</span></span>|<span data-ttu-id="68e9a-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68e9a-135">DateTimeOffset</span></span>||
|<span data-ttu-id="68e9a-136">dirSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="68e9a-136">dirSyncEnabled</span></span>|<span data-ttu-id="68e9a-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="68e9a-137">Boolean</span></span>|<span data-ttu-id="68e9a-138">**True** se esse objeto está sincronizado de um diretório local; **false** se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão).</span><span class="sxs-lookup"><span data-stu-id="68e9a-138">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="68e9a-139">displayName</span><span class="sxs-lookup"><span data-stu-id="68e9a-139">displayName</span></span>|<span data-ttu-id="68e9a-140">String</span><span class="sxs-lookup"><span data-stu-id="68e9a-140">String</span></span>|<span data-ttu-id="68e9a-141">O nome de exibição do locatário.</span><span class="sxs-lookup"><span data-stu-id="68e9a-141">The display name for the tenant.</span></span>|
|<span data-ttu-id="68e9a-142">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="68e9a-142">marketingNotificationEmails</span></span>|<span data-ttu-id="68e9a-143">String</span><span class="sxs-lookup"><span data-stu-id="68e9a-143">String</span></span>|                                        <span data-ttu-id="68e9a-144">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="68e9a-144">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="68e9a-145">objectType</span><span class="sxs-lookup"><span data-stu-id="68e9a-145">objectType</span></span>|<span data-ttu-id="68e9a-146">String</span><span class="sxs-lookup"><span data-stu-id="68e9a-146">String</span></span>|<span data-ttu-id="68e9a-p104">Uma cadeia de caracteres que identifica o tipo de objeto. Para locatários, o valor é sempre "Empresa". Herdado de [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="68e9a-p104">A string that identifies the object type. For tenants the value is always “Company”. Inherited from [directoryObject](../resources/directoryobject.md).</span></span>|
|<span data-ttu-id="68e9a-150">postalCode</span><span class="sxs-lookup"><span data-stu-id="68e9a-150">postalCode</span></span>|<span data-ttu-id="68e9a-151">String</span><span class="sxs-lookup"><span data-stu-id="68e9a-151">String</span></span>|            |
|<span data-ttu-id="68e9a-152">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="68e9a-152">preferredLanguage</span></span>|<span data-ttu-id="68e9a-153">String</span><span class="sxs-lookup"><span data-stu-id="68e9a-153">String</span></span>|            |
|<span data-ttu-id="68e9a-154">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="68e9a-154">provisionedPlans</span></span>|<span data-ttu-id="68e9a-155">ProvisionedPlan</span><span class="sxs-lookup"><span data-stu-id="68e9a-155">ProvisionedPlan</span></span>|                                        <span data-ttu-id="68e9a-156">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="68e9a-156">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="68e9a-157">provisioningErrors</span><span class="sxs-lookup"><span data-stu-id="68e9a-157">provisioningErrors</span></span>|<span data-ttu-id="68e9a-158">ProvisioningError</span><span class="sxs-lookup"><span data-stu-id="68e9a-158">ProvisioningError</span></span>|                                        <span data-ttu-id="68e9a-159">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="68e9a-159">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="68e9a-160">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="68e9a-160">securityComplianceNotificationMails</span></span>|<span data-ttu-id="68e9a-161">String</span><span class="sxs-lookup"><span data-stu-id="68e9a-161">String</span></span>||
|<span data-ttu-id="68e9a-162">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="68e9a-162">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="68e9a-163">String</span><span class="sxs-lookup"><span data-stu-id="68e9a-163">String</span></span>||
|<span data-ttu-id="68e9a-164">state</span><span class="sxs-lookup"><span data-stu-id="68e9a-164">state</span></span>|<span data-ttu-id="68e9a-165">String</span><span class="sxs-lookup"><span data-stu-id="68e9a-165">String</span></span>|            |
|<span data-ttu-id="68e9a-166">street</span><span class="sxs-lookup"><span data-stu-id="68e9a-166">street</span></span>|<span data-ttu-id="68e9a-167">String</span><span class="sxs-lookup"><span data-stu-id="68e9a-167">String</span></span>|            |
|<span data-ttu-id="68e9a-168">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="68e9a-168">technicalNotificationMails</span></span>|<span data-ttu-id="68e9a-169">String</span><span class="sxs-lookup"><span data-stu-id="68e9a-169">String</span></span>|                                        <span data-ttu-id="68e9a-170">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="68e9a-170">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="68e9a-171">telephoneNumber</span><span class="sxs-lookup"><span data-stu-id="68e9a-171">telephoneNumber</span></span>|<span data-ttu-id="68e9a-172">String</span><span class="sxs-lookup"><span data-stu-id="68e9a-172">String</span></span>|            |
|<span data-ttu-id="68e9a-173">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="68e9a-173">verifiedDomains</span></span>|<span data-ttu-id="68e9a-174">VerifiedDomain</span><span class="sxs-lookup"><span data-stu-id="68e9a-174">VerifiedDomain</span></span>|<span data-ttu-id="68e9a-p105">A coleção de domínios associados a este locatário.                            **Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="68e9a-p105">The collection of domains associated with this tenant.                            **Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="68e9a-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="68e9a-177">Response</span></span>

<span data-ttu-id="68e9a-178">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [organization](../resources/organization.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68e9a-178">If successful, this method returns a `200 OK` response code and updated [organization](../resources/organization.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="68e9a-179">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68e9a-179">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68e9a-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68e9a-180">Request</span></span>
<span data-ttu-id="68e9a-181">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68e9a-181">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/organization
Content-type: application/json
Content-length: 411

{
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "servicePlanId-value"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "country": "country-value",
  "countryLetterCode": "countryLetterCode-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="68e9a-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="68e9a-182">Response</span></span>
<span data-ttu-id="68e9a-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68e9a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "servicePlanId-value"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "country": "country-value",
  "countryLetterCode": "countryLetterCode-value",
  "displayName": "displayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
