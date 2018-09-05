# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="d8d9c-101">tipo de recurso onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="d8d9c-101">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="d8d9c-102">A propriedade **onPremisesExtensionAttributes** da entidade [usuário](user.md) contém quinze propriedades de extensão personalizada de atributo.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-102">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="d8d9c-103">Para um usuário **onPremisesSyncEnabled**, esse conjunto de propriedades é administrado no Active Directory local e sincronizado com o Azure AD, e é somente para leitura.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-103">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="d8d9c-104">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-104">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="d8d9c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8d9c-105">Properties</span></span>
| <span data-ttu-id="d8d9c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8d9c-106">Property</span></span>     | <span data-ttu-id="d8d9c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8d9c-107">Type</span></span>   |<span data-ttu-id="d8d9c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8d9c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8d9c-109">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="d8d9c-109">extensionAttribute1</span></span>|<span data-ttu-id="d8d9c-110">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8d9c-110">String</span></span>| <span data-ttu-id="d8d9c-111">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-111">First customizable extension attribute.</span></span> |
|<span data-ttu-id="d8d9c-112">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="d8d9c-112">extensionAttribute2</span></span>|<span data-ttu-id="d8d9c-113">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8d9c-113">String</span></span>| <span data-ttu-id="d8d9c-114">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-114">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="d8d9c-115">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="d8d9c-115">extensionAttribute3</span></span>|<span data-ttu-id="d8d9c-116">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8d9c-116">String</span></span>| <span data-ttu-id="d8d9c-117">Terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-117">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="d8d9c-118">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="d8d9c-118">extensionAttribute4</span></span>|<span data-ttu-id="d8d9c-119">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8d9c-119">String</span></span>| <span data-ttu-id="d8d9c-120">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-120">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="d8d9c-121">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="d8d9c-121">extensionAttribute5</span></span>|<span data-ttu-id="d8d9c-122">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8d9c-122">String</span></span>| <span data-ttu-id="d8d9c-123">Quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-123">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="d8d9c-124">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="d8d9c-124">extensionAttribute6</span></span>|<span data-ttu-id="d8d9c-125">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8d9c-125">String</span></span>| <span data-ttu-id="d8d9c-126">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-126">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="d8d9c-127">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="d8d9c-127">extensionAttribute7</span></span>|<span data-ttu-id="d8d9c-128">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8d9c-128">String</span></span>| <span data-ttu-id="d8d9c-129">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-129">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="d8d9c-130">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="d8d9c-130">extensionAttribute8</span></span>|<span data-ttu-id="d8d9c-131">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8d9c-131">String</span></span>| <span data-ttu-id="d8d9c-132">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-132">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="d8d9c-133">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="d8d9c-133">extensionAttribute9</span></span>|<span data-ttu-id="d8d9c-134">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8d9c-134">String</span></span>| <span data-ttu-id="d8d9c-135">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-135">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="d8d9c-136">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="d8d9c-136">extensionAttribute10</span></span>|<span data-ttu-id="d8d9c-137">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8d9c-137">String</span></span>| <span data-ttu-id="d8d9c-138">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-138">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="d8d9c-139">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="d8d9c-139">extensionAttribute11</span></span>|<span data-ttu-id="d8d9c-140">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8d9c-140">String</span></span>| <span data-ttu-id="d8d9c-141">Décimo primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-141">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="d8d9c-142">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="d8d9c-142">extensionAttribute12</span></span>|<span data-ttu-id="d8d9c-143">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8d9c-143">String</span></span>| <span data-ttu-id="d8d9c-144">Décimo segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-144">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="d8d9c-145">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="d8d9c-145">extensionAttribute13</span></span>|<span data-ttu-id="d8d9c-146">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8d9c-146">String</span></span>| <span data-ttu-id="d8d9c-147">Décimo terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-147">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="d8d9c-148">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="d8d9c-148">extensionAttribute14</span></span>|<span data-ttu-id="d8d9c-149">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8d9c-149">String</span></span>| <span data-ttu-id="d8d9c-150">Décimo quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-150">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="d8d9c-151">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="d8d9c-151">extensionAttribute15</span></span>|<span data-ttu-id="d8d9c-152">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8d9c-152">String</span></span>| <span data-ttu-id="d8d9c-153">Décimo quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="d8d9c-153">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d8d9c-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8d9c-154">JSON representation</span></span>

<span data-ttu-id="d8d9c-155">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d8d9c-155">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->