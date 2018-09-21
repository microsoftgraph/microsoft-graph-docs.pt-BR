# <a name="get-outlook-contacts-in-a-shared-folder"></a>Obtenha os contatos do Outlook em uma pasta compartilhada

O Outlook permite que os clientes compartilhem pastas entre si e forneçam acesso de "leitura", "criação", "modificação" ou "exclusão" para pastas de contato individuais. O Outlook também permite que um cliente delegue outro usuário para agir em seu nome e acessar pastas específicas ou toda a caixa de correio dele; Isso também é conhecido como "delegação" no Outlook.

Via programação, o Microsoft Graph oferece suporte para obter contatos em pastas de contatos compartilhadas por outros usuários, além de obter as próprias pastas compartilhadas. O suporte também se aplica a pastas em uma caixa de correio delegada.

Por exemplo, Garth compartilhou com John uma pasta de contato personalizada com acesso de leitura. Se John estiver conectado no seu aplicativo e tiver fornecido permissões delegadas (Contacts.Read.Shared ou Contacts.ReadWrite.Shared), o seu aplicativo poderá acessar a pasta de contatos personalizada do Garth e os contatos nela contidos, conforme descrito abaixo.

## <a name="get-a-contact-in-the-shared-folder"></a>Obter um contato na pasta compartilhada

Você pode obter um contato específico na pasta de contato personalizada que Garth compartilhou com John:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

Após a conclusão bem-sucedida, você obterá HTTP 200 OK e a instância [contact](../api-reference/v1.0/resources/contact.md) identificada por `{id}` da pasta de contatos compartilhada por Garth.

## <a name="get-all-contacts-in-the-shared-folder"></a>Obter todos os contatos na pasta compartilhada

Obtenha todos os contatos na pasta de contatos compartilhada por Garth:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

Após a conclusão bem-sucedida, você obterá HTTP 200 OK e uma coleção de instâncias [contact](../api-reference/v1.0/resources/contact.md) na pasta de contatos compartilhada por Garth.

## <a name="get-the-shared-folder"></a>Obter a pasta compartilhada

Obtenha a pasta de contatos que Garth compartilhou com John.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

Após a conclusão bem-sucedida, você obterá HTTP 200 OK e uma instância [contactFolder](../api-reference/v1.0/resources/contactfolder.md) que representa a pasta de contatos compartilhada por Garth.

Os mesmos recursos GET aplicam se Garth delegadar a John sua caixa de correio inteira.

Se Garth não tiver compartilhado a pasta de contatos com John, nem delegado sua caixa de correio, especificar a identificação de usuário de Garth ou nome UPN nessas operações GET retornará um erro. 


## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Por que se integrar aos contatos pessoais do Outlook](outlook-contacts-concept-overview.md)
- A [API de Contatos](../api-reference/v1.0/resources/contact.md) no Microsoft Graph v 1.0.