# <a name="update-organization"></a><span data-ttu-id="b983e-101">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="b983e-101">Update organization</span></span>

<span data-ttu-id="b983e-102">Atualize as propriedades da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="b983e-102">Update the properties of the currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="b983e-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b983e-103">Permissions</span></span>

<span data-ttu-id="b983e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b983e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b983e-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b983e-106">Permission type</span></span>      | <span data-ttu-id="b983e-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b983e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b983e-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b983e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b983e-109">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b983e-109">Not supported.</span></span>    |
|<span data-ttu-id="b983e-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b983e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b983e-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b983e-111">Not supported.</span></span>    |
|<span data-ttu-id="b983e-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b983e-112">Application</span></span> | <span data-ttu-id="b983e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b983e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b983e-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b983e-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization

```

## <a name="request-headers"></a><span data-ttu-id="b983e-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b983e-115">Request headers</span></span>

| <span data-ttu-id="b983e-116">Nome</span><span class="sxs-lookup"><span data-stu-id="b983e-116">Name</span></span>       | <span data-ttu-id="b983e-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="b983e-117">Type</span></span> | <span data-ttu-id="b983e-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="b983e-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b983e-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="b983e-119">Authorization</span></span>  | <span data-ttu-id="b983e-120">string</span><span class="sxs-lookup"><span data-stu-id="b983e-120">string</span></span>  | <span data-ttu-id="b983e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b983e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b983e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b983e-123">Request body</span></span>
<span data-ttu-id="b983e-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="b983e-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b983e-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="b983e-125">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="b983e-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b983e-126">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b983e-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b983e-127">Property</span></span>     | <span data-ttu-id="b983e-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="b983e-128">Type</span></span>   |<span data-ttu-id="b983e-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b983e-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b983e-130">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="b983e-130">assignedPlans</span></span>|<span data-ttu-id="b983e-131">AssignedPlan</span><span class="sxs-lookup"><span data-stu-id="b983e-131">AssignedPlan</span></span>|<span data-ttu-id="b983e-132">A coleção de planos de serviço associados ao locatário.</span><span class="sxs-lookup"><span data-stu-id="b983e-132">The collection of service plans associated with the tenant. Not nullable.</span></span> <span data-ttu-id="b983e-133">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="b983e-133">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="b983e-134">cidade</span><span class="sxs-lookup"><span data-stu-id="b983e-134">city</span></span>|<span data-ttu-id="b983e-135">String</span><span class="sxs-lookup"><span data-stu-id="b983e-135">String</span></span>|            |
|<span data-ttu-id="b983e-136">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="b983e-136">companyLastDirSyncTime</span></span>|<span data-ttu-id="b983e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b983e-137">DateTimeOffset</span></span>|<span data-ttu-id="b983e-138">A hora e a data em que o locatário foi sincronizado pela última vez com o diretório no local.</span><span class="sxs-lookup"><span data-stu-id="b983e-138">The time and date at which the tenant was last synced with the on-premise directory.</span></span>|
|<span data-ttu-id="b983e-139">country</span><span class="sxs-lookup"><span data-stu-id="b983e-139">country</span></span>|<span data-ttu-id="b983e-140">String</span><span class="sxs-lookup"><span data-stu-id="b983e-140">String</span></span>|            |
|<span data-ttu-id="b983e-141">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="b983e-141">countryLetterCode</span></span>|<span data-ttu-id="b983e-142">String</span><span class="sxs-lookup"><span data-stu-id="b983e-142">String</span></span>|            |
|<span data-ttu-id="b983e-143">deletionTimestamp</span><span class="sxs-lookup"><span data-stu-id="b983e-143">deletionTimestamp</span></span>|<span data-ttu-id="b983e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b983e-144">DateTimeOffset</span></span>||
|<span data-ttu-id="b983e-145">dirSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="b983e-145">dirSyncEnabled</span></span>|<span data-ttu-id="b983e-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="b983e-146">Boolean</span></span>|<span data-ttu-id="b983e-147">**True** se esse objeto está sincronizado de um diretório local; **false** se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão).</span><span class="sxs-lookup"><span data-stu-id="b983e-147">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="b983e-148">displayName</span><span class="sxs-lookup"><span data-stu-id="b983e-148">displayName</span></span>|<span data-ttu-id="b983e-149">String</span><span class="sxs-lookup"><span data-stu-id="b983e-149">String</span></span>|<span data-ttu-id="b983e-150">O nome de exibição do locatário.</span><span class="sxs-lookup"><span data-stu-id="b983e-150">The display name for the tenant.</span></span>|
|<span data-ttu-id="b983e-151">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="b983e-151">marketingNotificationEmails</span></span>|<span data-ttu-id="b983e-152">String</span><span class="sxs-lookup"><span data-stu-id="b983e-152">String</span></span>|                                        <span data-ttu-id="b983e-153">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="b983e-153">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="b983e-154">objectType</span><span class="sxs-lookup"><span data-stu-id="b983e-154">objectType</span></span>|<span data-ttu-id="b983e-155">String</span><span class="sxs-lookup"><span data-stu-id="b983e-155">String</span></span>|<span data-ttu-id="b983e-156">Uma cadeia de caracteres que identifica o tipo de objeto.</span><span class="sxs-lookup"><span data-stu-id="b983e-156">A string that identifies the object type. For tenants the value is always “Company”.</span></span> <span data-ttu-id="b983e-157">Para locatários, o valor é sempre "Empresa".</span><span class="sxs-lookup"><span data-stu-id="b983e-157">A string that identifies the object type. For tenants the value is always “Company”.</span></span> <span data-ttu-id="b983e-158">Herdado de [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="b983e-158">Inherited from [directoryObject](../resources/directoryobject.md).</span></span>|
|<span data-ttu-id="b983e-159">postalCode</span><span class="sxs-lookup"><span data-stu-id="b983e-159">postalCode</span></span>|<span data-ttu-id="b983e-160">String</span><span class="sxs-lookup"><span data-stu-id="b983e-160">String</span></span>|            |
|<span data-ttu-id="b983e-161">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="b983e-161">preferredLanguage</span></span>|<span data-ttu-id="b983e-162">String</span><span class="sxs-lookup"><span data-stu-id="b983e-162">String</span></span>|            |
|<span data-ttu-id="b983e-163">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="b983e-163">provisionedPlans</span></span>|<span data-ttu-id="b983e-164">ProvisionedPlan</span><span class="sxs-lookup"><span data-stu-id="b983e-164">ProvisionedPlan</span></span>|                                        <span data-ttu-id="b983e-165">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="b983e-165">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="b983e-166">provisioningErrors</span><span class="sxs-lookup"><span data-stu-id="b983e-166">provisioningErrors</span></span>|<span data-ttu-id="b983e-167">ProvisioningError</span><span class="sxs-lookup"><span data-stu-id="b983e-167">ProvisioningError</span></span>|                                        <span data-ttu-id="b983e-168">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="b983e-168">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="b983e-169">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="b983e-169">securityComplianceNotificationMails</span></span>|<span data-ttu-id="b983e-170">String</span><span class="sxs-lookup"><span data-stu-id="b983e-170">String</span></span>||
|<span data-ttu-id="b983e-171">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="b983e-171">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="b983e-172">String</span><span class="sxs-lookup"><span data-stu-id="b983e-172">String</span></span>||
|<span data-ttu-id="b983e-173">state</span><span class="sxs-lookup"><span data-stu-id="b983e-173">state</span></span>|<span data-ttu-id="b983e-174">String</span><span class="sxs-lookup"><span data-stu-id="b983e-174">String</span></span>|            |
|<span data-ttu-id="b983e-175">street</span><span class="sxs-lookup"><span data-stu-id="b983e-175">street</span></span>|<span data-ttu-id="b983e-176">String</span><span class="sxs-lookup"><span data-stu-id="b983e-176">String</span></span>|            |
|<span data-ttu-id="b983e-177">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="b983e-177">technicalNotificationMails</span></span>|<span data-ttu-id="b983e-178">String</span><span class="sxs-lookup"><span data-stu-id="b983e-178">String</span></span>|                                        <span data-ttu-id="b983e-179">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="b983e-179">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="b983e-180">telephoneNumber</span><span class="sxs-lookup"><span data-stu-id="b983e-180">telephoneNumber</span></span>|<span data-ttu-id="b983e-181">String</span><span class="sxs-lookup"><span data-stu-id="b983e-181">String</span></span>|            |
|<span data-ttu-id="b983e-182">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="b983e-182">verifiedDomains</span></span>|<span data-ttu-id="b983e-183">VerifiedDomain</span><span class="sxs-lookup"><span data-stu-id="b983e-183">VerifiedDomain</span></span>|<span data-ttu-id="b983e-184">A coleção de domínios associados a este locatário.</span><span class="sxs-lookup"><span data-stu-id="b983e-184">The collection of domains associated with this tenant. Not nullable.</span></span> <span data-ttu-id="b983e-185">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="b983e-185">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="b983e-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="b983e-186">Response</span></span>

<span data-ttu-id="b983e-187">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [organization](../resources/organization.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b983e-187">If successful, this method returns a `200 OK` response code and updated [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b983e-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b983e-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="b983e-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b983e-189">Request</span></span>

<span data-ttu-id="b983e-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b983e-190">Here is an example of the request.</span></span>

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

<br/>

### <a name="response"></a><span data-ttu-id="b983e-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="b983e-191">Response</span></span>

<span data-ttu-id="b983e-192">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b983e-192">Here is an example of the response.</span></span> <span data-ttu-id="b983e-193">**Observação**: o objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="b983e-193">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b983e-194">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b983e-194">All default properties will be returned from the actual call.</span></span>

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

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
