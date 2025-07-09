# ⛽️ Álcool ou Gasolina – App Comparador de Combustível

> Aplicativo Android simples que ajuda a decidir se compensa abastecer com **álcool (etanol)** ou **gasolina** com base no preço informado.

![Badge Kotlin](https://img.shields.io/badge/Kotlin-1.9.x-purple?logo=kotlin)
![Badge Android](https://img.shields.io/badge/Android-API%2024%2B-green?logo=android)

---

## 🚀 Funcionalidades

- Entrada de preço do **álcool** (R$)
- Entrada de preço da **gasolina** (R$)
- Botão **Calcular** que:
  - Se `álcool / gasolina` < **0.7** → recomenda **Álcool**
  - Caso contrário → recomenda **Gasolina**
- Mensagem dinâmica exibindo a melhor escolha
- Layout simples com **ViewBinding**

---

## 🏗️ Tecnologias & Conceitos

| Camada | Tech / Lib | Observação |
|--------|------------|------------|
| UI | **ViewBinding** | Acesso type-safe aos componentes |
| Lógica | Kotlin 1.9.x | Operadores, if/else, formatação `String.format()` |
| Build | Gradle Kotlin DSL (7+) | Script simplificado |

---

## 🎯 Pré-requisitos

- **Android Studio Giraffe** ou superior
- JDK 17
- Emulador ou dispositivo **API 24+**

---

## ⚙️ Execução

```bash
# Clone o repositório
$ git clone https://github.com/Lari30/AulaAppAlcoolOuGasolina.git
$ cd AlcoolOuGasolina

# Abra no Android Studio e clique em ▶️
```

> Se preferir via terminal:
>
> ```bash
> ./gradlew installDebug && adb shell monkey -p com.seu.package 1
> ```

---

## 🧪 Testes (Opcional)

Projeto simples, mas você pode adicionar:

- **JUnit** para testar função `calcularMelhorCombustivel()`
- **Espresso** para validar fluxo de UI

```kotlin
fun calcularMelhorCombustivel(alcool: Double, gasolina: Double): String =
    if (alcool/gasolina < 0.7) "Álcool" else "Gasolina"
```

---

## 🛣️ Roadmap

- [ ] Migrar layout para **Jetpack Compose**
- [ ] Adicionar **Theme Material3**
- [ ] Internacionalização (EN, PT-BR)
- [ ] Teste unitário + CI GitHub Actions

---

## 🤝 Contribuindo

1. Fork este repositório
2. Crie sua branch: `git checkout -b feature/melhorias`
3. Commit: `git commit -m 'feat: melhoria x'`
4. Push: `git push origin feature/melhorias`
5. Abra um Pull Request

---

## 📄 Licença

Este projeto está sob a licença MIT – veja o arquivo **LICENSE** para detalhes.

---

### Autor

Feito por **Larissa Santos** • [LinkedIn](https://www.linkedin.com/in/larissa-santos-478961ab/) • contato: larynha_santos@yahoo.com.br
